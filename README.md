# unfocus
> An accessible way of removing :focus outline on click.

[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md) [![npm](https://img.shields.io/npm/v/unfocus.svg?style=flat-square)](https://www.npmjs.com/package/unfocus) [![npm](https://img.shields.io/npm/dt/unfocus.svg?style=flat-square)](https://www.npmjs.com/package/unfocus)

## Intro
Accessibility on the web is very important and when you have to make the decision between accessibility and style, I urge you to always choose accessibility. That said, sometimes there is a way to make something accessible with style, and this package tries to help you. The idea is to keep the default `outline` on `:focus` (or any alternative highlight on `:focus`) but remove it when the user actually clicks on an item, as the highlight is needed for keyboard navigation only.

## Installation

### via npm
```
npm install unfocus --save
```

### via bower
```
bower install unfocus --save
```

## API
By default the following style will be applied.

```css
:focus{
    outline: none !important;
}
```

However, you can change the style that is applied to `:focus` by passing anything to the `.style` method. This will be automatically added to the `:focus` style, that is used to hide the highlight on click.

```javascript
unfocus.style('box-shadow: none !important;');
```
