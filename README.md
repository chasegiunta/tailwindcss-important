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

The important plugin exposes an `important` variant for you to use by prepending `!` to your class names: `!text-white hover:!bg-black`

```js
  plugins: [
    require('tailwindcss-important')(),
  ],
```

```js
  variants: {
    extend: {
      textColors: ['responsive', 'hover', 'important'],
    }
  }
```

### Purgecss
If you're using purgecss, you'll want to update your TailwindExtractor to include `!`.
```
content.match(/[A-Za-z0-9-_:!\/]+/g) || [];
```
