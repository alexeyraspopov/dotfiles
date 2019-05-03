# Frontend Dotfiles

This repository is a collection of config files for top level frontend tools.

## Babel Plugins

### [babel-plugin-auto-import](https://github.com/PavelDymkov/babel-plugin-auto-import)

I use this plugin because I got tired of broken feedback cycle where I need to
go back to code to fix it after I used a hook that wasn't previously imported.
The plugin adds necessary import declarations in the build time.

### [babel-plugin-module-resolver](https://github.com/tleunen/babel-plugin-module-resolver)

Allows to get rid of `../../../module` in imports without relying on a bundler
tool of choice. Root folders and specific aliases can be defined. Paths are
resolved in the build time. Perfect option for both Webpack and Parcel.

### [babel-plugin-style-literal](https://github.com/alexeyraspopov/babel-plugin-style-literal)

I use inline styles to make prototyping process faster. Also data visualization
requires dynamic styles that remain in JSX. Using JS object for styles is
frustrating and introduce a lot of friction. This plugin allows writing CSS
code that is converted to JS object in the build time.

## ESLint Plugins

### [eslint-plugin-react](https://github.com/yannickcr/eslint-plugin-react)

A set of custom rules to improve React/JSX integration with ESLint.

### [eslint-plugin-react-hooks](https://github.com/facebook/react/tree/master/packages/eslint-plugin-react-hooks)

A set of custom rules provided by React team to enhance the developer experience
in using hooks.
