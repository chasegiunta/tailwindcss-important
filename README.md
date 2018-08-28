# !important Tailwind Plugin

## Installation

Add this plugin to your project:

```bash
# Install via npm
npm install --save-dev tailwindcss-important

# Install via yarn
yarn add tailwindcss-important --dev
```

Adding variants through plugins is currently an experimental feature in tailwind and requires version 0.6.2 or higher.

## Usage

The important plugin exposes an `important` variant for you to use by prepending `!` to your class names: `!text-white !bg-black`

```js
require('tailwindcss-important')()
```

```js
textColors: ['responsive', 'hover', 'important'],
```

```js
experiments: {
  pluginVariants: true
}
```