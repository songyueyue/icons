<p align="center">
  <a href="https://uiw-react.github.io/icons">
    <img width="150" src="https://raw.githubusercontent.com/uiw-react/uiw/master/docs/assets/logo-README.svg?sanitize=true">
  </a>
</p>


Icon Font
---


[![](https://img.shields.io/github/issues/uiw-react/icons.svg)](https://github.com/uiw-react/icons/issues) [![](https://img.shields.io/github/forks/uiw-react/icons.svg)](https://github.com/uiw-react/icons/network) [![](https://img.shields.io/github/stars/uiw-react/icons.svg)](https://github.com/uiw-react/icons/stargazers) [![](https://img.shields.io/github/release/uiw-react/icons.svg)](https://github.com/uiw-react/icons/releases) [![Packagist](https://img.shields.io/dub/l/vibe-d.svg)](https://github.com/uiw-react/icons) [![Packagist](https://img.shields.io/npm/v/uiw-iconfont.svg)](https://www.npmjs.com/package/uiw-iconfont)

The premium icon font for  uiw Component Library. Designed by [@liwen0526](https://github.com/liwen0526). 

Visit **[https://uiw-react.github.io/icons/](https://uiw-react.github.io/icons/)** and check out the search feature, which has keywords identifying common icon names and styles. For example, if you search for "arrow" we call up every icon that could possibly be used as an arrow. We've also included each icon's class name for easy copy / pasting when you're developing!

They are free to use and licensed under [MIT](https://opensource.org/licenses/MIT). We intend for this icon pack to be used with [uiw](https://uiw-react.github.io), but it’s by no means limited to it. Use them wherever you see fit, personal or commercial. 

<p align="center">
  <a href="https://uiw-react.github.io/icons">
    <img src="https://github.com/uiw-react/icons/raw/master/build/assets/uiw-font.png">
  </a>
</p>

## Installation

```bash
npm install uiw-iconfont --save
```

## HTML Example

You can use [https://uiw-react.github.io/icons/](https://uiw-react.github.io/icons/) to easily find the icon you want to use. Once you've copied the desired icon's CSS classname, simply add the icon and icon's classname, such as `apple` to an HTML element.

You need link CSS

```html
<link rel="stylesheet" type="text/css" href="node_modules/fonts/w-iconfont.css">
```

Used in Less:

```css
@import "~uiw-iconfont/fonts/w-iconfont.css";
```

Used in JS:

```js
import 'uiw-iconfont/fonts/w-iconfont.css';
// or
import 'uiw-iconfont/fonts/w-iconfont.less';
```

note: It has a `w-icon-` prefix. 

```html
<i class="w-icon-apple"></i>
```

Or use the `Unicode`, You can use [Unicode website](https://uiw-react.github.io/icons/unicode.html) to easily find the `Unicode` icon you want to use. 

```html
<style>
.iconfont{
  font-family: "w-iconfont" !important;
  font-size: 16px;
  font-style: normal;
  -webkit-font-smoothing: antialiased;
  -webkit-text-stroke-width: 0.2px;
  -moz-osx-font-smoothing: grayscale;
}
</style>
<span class="iconfont">&#59907;</span>
```

**In Webpack**

```js
{
  test: /w-iconfont\.(eot|ttf|svg)$/,
  use: [
    {
      loader: require.resolve('url-loader'),
      options: { limit: 8192 }
    },
    {
      loader: require.resolve('file-loader'),
      options: {
        name: 'static/fonts/[name].[hash:8].[ext]',
      }
    }
  ]
},
```

## Development

Run the `npm install` to install the dependencies after cloning the project and you'll be able to:

To build `*.svg` `*.ttf` `*.woff` `*.eot` files

```bash
npm run font
```

To build site and push gh-pages branch

```bash
npm run start
```

## License

Licensed under the [MIT License](https://opensource.org/licenses/MIT).