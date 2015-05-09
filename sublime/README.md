# Sublime Text

## Packages

- [Alignment](https://packagecontrol.io/packages/Alignment)
- [AngularJS](https://packagecontrol.io/packages/AngularJS)
- [Babel](https://packagecontrol.io/packages/Babel)
- [Babel Snippets](https://packagecontrol.io/packages/Babel%20Snippets)
- [BracketHighlighter](https://packagecontrol.io/packages/BracketHighlighter)
- [DocBlockr](https://packagecontrol.io/packages/DocBlockr)
- [Emmet](https://packagecontrol.io/packages/Emmet)
- [GitGutter](https://packagecontrol.io/packages/GitGutter)
- [HTML5](https://packagecontrol.io/packages/HTML5)
- [JavaScript & NodeJS Snippets](https://packagecontrol.io/packages/JavaScript%20%26%20NodeJS%20Snippets)
- [jQuery](http://packagecontrol.io/packages/jQuery)
- [JsFormat](https://packagecontrol.io/packages/JsFormat)
- [LESS](https://packagecontrol.io/packages/LESS)
- [Predawn](https://packagecontrol.io/packages/Predawn)
- [Sass](https://packagecontrol.io/packages/Sass)
- [SideBarEnhancements](https://packagecontrol.io/packages/SideBarEnhancements)
- [SublimeLinter](https://packagecontrol.io/packages/SublimeLinter)
  - [SublimeLinter-eslint](https://packagecontrol.io/packages/SublimeLinter-contrib-eslint)
  - [SublimeLinter-json](https://packagecontrol.io/packages/SublimeLinter-json)
  - [SublimeLinter-php](https://packagecontrol.io/packages/SublimeLinter-php)
  - [SublimeLinter-scss-lint](https://packagecontrol.io/packages/SublimeLinter-contrib-scss-lint)
- [Theme - Afterglow](https://packagecontrol.io/packages/Theme%20-%20Afterglow)

## Preferences & Keybindings

Move any files with a `.sublime-` extension to the `/Packages/User` directory in your Sublime Text 3 settings directory (on OSX, `~/Library/Application Support/Sublime Text 3`)

Some keybindings have been changed to avoid conflicts between Packages:

- Change **Alignment** keybinding as it conflicts with a SublimeLinter shortcut.

## Babel

Let's write ES6!

Ensure that the syntax of all `.js` and `.jsx` files is **JavaScript (Babel)**

To do this, open a `.js` file and a `.jsx` file, and for each of them, go to *View > Syntax > Open all with current extension as ... > Babel > JavaScript (Babel)*

## SublimeLinter

Install all the SublimeLinter packages last (it copies your current color scheme and modifies it).

For JavaScript linting with Babel + ESLint, the `.eslintrc` file in the `sublime/` directory should be copied to your project root (taken from the [Airbnb JavaScript style guide](https://github.com/airbnb/javascript)).

User settings have been modified to use ESLint on files with the "JavaScript (Babel)" syntax.