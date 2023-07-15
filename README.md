# flipper-plugin-reanimated

This is a plugin for the [Flipper](https://github.com/facebook/flipper) debugging
tool, which allows for debugging React Native apps using the Reanimated package.

It is mainly based on the hermesdebuggerrn plugin that is bundled with Flipper,
but with a few minor changes that are needed for our use-case.

*This version of the plugin is based on https://github.com/facebook/flipper/commit/c8776175c34d2574c7ee056bbf3c4d26dc9332be

## Development

1. Clone the repo and run `yarn` in the project root

2. **While Flipper is closed** go to `~/.flipper/config.json` and add the
folder containing the repo folder to the `pluginPaths` array.

Example:

Your file structure looks like this:
```
~/flipper-plugins/
    |
    - flipper-plugin-reanimated/
```

Then you should add the `flipper-plugins` folder to the `pluginPaths` array.

**Warning!** *Remember to add the absolute path to `pluginPaths`.*

3. Run `yarn watch` which will build the plugin and watch for changes later

4. Open Flipper and the plugin should be visible in the plugin list
