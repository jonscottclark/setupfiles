# Sublime Text

## Packages

You'll need to install [Package Control](https://packagecontrol.io/installation) before adding any of these plugins.

- [Alignment](https://packagecontrol.io/packages/Alignment)
- [AngularJS](https://packagecontrol.io/packages/AngularJS)
- [Babel](https://packagecontrol.io/packages/Babel)
- [Babel Snippets](https://packagecontrol.io/packages/Babel%20Snippets)
- [BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter)
- [Color Highlighter](https://packagecontrol.io/packages/Color%20Highlighter)
- [DocBlockr](https://packagecontrol.io/packages/DocBlockr)
- [EditorConfig](https://packagecontrol.io/packages/EditorConfig)
- [Emmet](https://packagecontrol.io/packages/Emmet)
- [GitGutter](https://packagecontrol.io/packages/GitGutter)
- [HTML5](https://packagecontrol.io/packages/HTML5)
- [Jade](https://packagecontrol.io/packages/Jade)
- [JavaScript & NodeJS Snippets](https://packagecontrol.io/packages/JavaScript%20%26%20NodeJS%20Snippets)
- [jQuery](http://packagecontrol.io/packages/jQuery)
- [JsFormat](https://packagecontrol.io/packages/JsFormat)
- [LESS](https://packagecontrol.io/packages/LESS)
- [Sass](https://packagecontrol.io/packages/Sass)
- [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)
- [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)
  - [SublimeLinter-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)
  - [SublimeLinter-json](https://packagecontrol.io/packages/SublimeLinter-json)
  - [SublimeLinter-php](https://packagecontrol.io/packages/SublimeLinter-php)
  - [SublimeLinter-scss-lint](https://packagecontrol.io/packages/SublimeLinter-contrib-scss-lint)
- [Theme - Afterglow](https://packagecontrol.io/packages/Theme%20-%20Afterglow)

## Theme & Appearance

Set the colour scheme by selecting *Preferences > Color Scheme > Theme - Afterglow* and picking the variation of your choice.

The option to load the theme itself is included in the Preferences file.

## Preferences & Keybindings

Move any files with a `.sublime-` extension in this directory to the `/Packages/User` directory in your Sublime Text 3 settings directory (on OSX, `~/Library/Application Support/Sublime Text 3`).

Some keybindings have been changed to avoid conflicts between Packages:

- Changed the default **Alignment** keybinding `⌘ + Ctrl + A` as it conflicts with a the SublimeLinter shortcut to *Show All Errors*. Now, use `⌘ + ⌥ + Shift + A`; just a personal preference, same hand pattern as *Save for web* in Photoshop :)

## Babel

Let's write ES6!

Ensure that the syntax of all `.js` and `.jsx` files is **JavaScript (Babel)**

To do this, open a `.js` file and a `.jsx` file, and for each of them, go to *View > Syntax > Open all with current extension as ... > Babel > JavaScript (Babel)*

## SublimeLinter

For JavaScript linting with Babel + ESLint, the SublimeLinter settings have been modified to invoke ESLint on files with the "JavaScript (Babel)" syntax.

To define linting rules, make sure you have an appropriate `.eslintrc` file in the root directory of each ES6 project (you can find a thoroughly documented `.eslintrc` in the [Airbnb JavaScript style guide](https://github.com/airbnb/javascript)).