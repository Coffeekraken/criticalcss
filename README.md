# Coffeekraken criticalcss <img src=".resources/coffeekraken-logo.jpg" height="25px" />

<p>
	<!-- <a href="https://travis-ci.org/coffeekraken/criticalcss">
		<img src="https://img.shields.io/travis/coffeekraken/criticalcss.svg?style=flat-square" />
	</a> -->
	<a href="https://www.npmjs.com/package/coffeekraken-criticalcss">
		<img src="https://img.shields.io/npm/v/coffeekraken-criticalcss.svg?style=flat-square" />
	</a>
	<a href="https://github.com/coffeekraken/criticalcss/blob/master/LICENSE.txt">
		<img src="https://img.shields.io/npm/l/coffeekraken-criticalcss.svg?style=flat-square" />
	</a>
	<!-- <a href="https://github.com/coffeekraken/criticalcss">
		<img src="https://img.shields.io/npm/dt/coffeekraken-criticalcss.svg?style=flat-square" />
	</a>
	<a href="https://github.com/coffeekraken/criticalcss">
		<img src="https://img.shields.io/github/forks/coffeekraken/criticalcss.svg?style=social&label=Fork&style=flat-square" />
	</a>
	<a href="https://github.com/coffeekraken/criticalcss">
		<img src="https://img.shields.io/github/stars/coffeekraken/criticalcss.svg?style=social&label=Star&style=flat-square" />
	</a> -->
	<a href="https://twitter.com/coffeekrakenio">
		<img src="https://img.shields.io/twitter/url/http/coffeekrakenio.svg?style=social&style=flat-square" />
	</a>
	<a href="http://coffeekraken.io">
		<img src="https://img.shields.io/twitter/url/http/shields.io.svg?style=flat-square&label=coffeekraken.io&colorB=f2bc2b&style=flat-square" />
	</a>
</p>

Simply and quickly generate the critical css depending on a list of pages to take as source.

## Table of content

1. [Install](#readme-install)
2. [Get Started](#readme-get-started)
3. [CLI Options](#readme-cli-options)
4. [`pages.json`](#readme-pagesjson)
5. [Contribute](#readme-contribute)
6. [Who are Coffeekraken?](#readme-who-are-coffeekraken)
7. [Licence](#readme-license)

<a name="readme-install"></a>
## Install

```
npm install coffeekraken-criticalcss --save-dev
```

<a name="readme-get-started"></a>
## Get Started

Use the CLI as follow:

```
coffeekraken-criticalcss -o dist/css/critical.css -c dist/css/style.css
```

<a name="readme-cli-options"></a>
## CLI Options

Here's all the CLI options available:

### `-o|--output`

Output critical css file

- default : `dist/css/critical.css`

### `-c|--css`

Css file to use to generate critical one

- default : `dist/css/style.css`

### `-p|--pages`

List of pages urls to process (space separated).
By default, it would try to find a `pages.json` file in your project root folder, then it would try to find a `pages` property in your `package.json`. See bellow for more info on that.

- default : `null`

### `-h|--host`

Hostname on which to make pages requests

- default : `http://localhost:8080`

### `-w|--width`

Width of the viewport to calculate the critical css

- default : `1200`

### `-h|--height`

Height of the viewport to calculate the critical css

- default : `900`

<a id="readme-pagesjson"></a>
## `pages.json`

You can create a `pages.json` file at your project root folder that will be used to generate the critical css from the pages url defined here.
Here's a sample pages.json file:

```json
{
  "home": {
    "title": "Homepage",
    "url": "/"
  },
  "contact": {
    "title": "Contact",
    "url": "/contact"
  }
}
```

> You can if you prefere have the same structure in your `package.json` file under a `pages` property.

<a id="readme-contribute"></a>
## Contribute

This is an open source project and will ever be! You are more that welcomed to contribute to his development and make it more awesome every day.
To do so, you have several possibilities:

1. [Share the love ❤️](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md#contribute-share-the-love)
2. [Declare issues](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md#contribute-declare-issues)
3. [Fix issues](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md#contribute-fix-issues)
4. [Add features](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md#contribute-add-features)
5. [Build web component](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md#contribute-build-web-component)

<a id="readme-who-are-coffeekraken"></a>
## Who are Coffeekraken

We try to be **some cool guys** that build **some cool tools** to make our (and yours hopefully) **every day life better**.  

#### [More on who we are](https://github.com/Coffeekraken/coffeekraken/blob/master/who-are-we.md)

<a id="readme-license"></a>
## License

The code is available under the [MIT license](LICENSE.txt). This mean that you can use, modify, or do whatever you want with it. This mean also that it is shipped to you for free, so don't be a hater and if you find some issues, etc... feel free to [contribute](https://github.com/Coffeekraken/coffeekraken/blob/master/contribute.md) instead of sharing your frustrations on social networks like an asshole...
