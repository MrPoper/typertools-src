# React Starter Plugin

This plugin is a good place to get started when building a Photoshop plugin using React. It comes defined with all the dependencies that you'll need to get started. As this is a React project, you'll need to do some initial configuration before this will be usable in Photoshop.

## Install dependencies

First, make sure that `yarn` is installed on your system.

```
npm install -g yarn
```

Then, after you ensure that your terminal is in the root of this project, use `yarn` to install the various dependencies needed:

```
yarn install
```

## Build Process

There are two ways to build the plugin for use in Photoshop:

* `yarn watch` will build a development version of the plugin, and recompile everytime you make a change to the source files. The result is placed in `dist` folder. 
* `yarn build` will build a production version of the plugin and place it in `dist` folder. It will not update every time you make a change to the source files.

> You **must** run either `watch` or `build` prior to trying to use within Photoshop!

## Launching in Photoshop

You can use the UXP Developer Tools to load the plugin into Photoshop.

If the plugin hasn't already been added to your workspace in the UXP Developer Tools, you can add it by clicking "Add Plugin...". You can either add the `dist` folder or the `plugin` folder - if you add the plugin folder - then you need to set the relative path to build folder ( 'dist' ) in the Plugin's Load Option.

Once added, you can load it into Photoshop by clicking the ••• button on the corresponding row, and clicking "Load". Switch to Photoshop and you should see the starter panels.

## What this plugin does

This plugin doesn't do much, but does illustrate how to create two panels in Photoshop with `entrypoints.setup`, and how to create flyout menus. It also demonstrates the use of several Spectrum UXP widgets to create a simple color picker in the primary panel.

