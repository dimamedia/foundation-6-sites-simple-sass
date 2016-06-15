# Purified Foundation for Sites 6

## Foundation?

Foundation is the most advanced responsive front-end framework in the world. Quickly go from prototype to production, building sites or apps that work on any kind of device with Foundation. Includes a fully customizable, responsive grid, a large library of Sass mixins, commonly used JavaScript plugins, and full accessibility support.

## Purified?

Cleaned Foundation-sites 6 from all dependencies. Pure scss base for compiling with user's preferred sass compiler.
Separated javascript files to combine only needed features with user's preferred script loader or combiner minifier.

Motion-ui and What-input is included to this pack and can be used if needed.

### Foundation version?

This repository forked from zurb/foundation-sites while version 6.2.3.

## Getting Started

Download or clone this package.

### Manual config setup

- Use `scss/app.scss` to select required foundation features and add own stuff.
 - Set `$flex: true;` to enable flexbox-mode.
- Edit `scss/_settings.scss` to modify foundation elements.
 - If RTL mode required set `$global-text-direction: rtl;`
- Compile with preferred [sass](http://sass-lang.com/install) compiler.

### Documentation

The documentation can be found at <https://foundation.zurb.com/sites/docs>.

## Javascript files

### Jquery

There is several versions of jquery to choose:
- Jquery standard `jquery.js` or `jquery.min.js`
- Jquery slim `jquery.slim.js` or `jquery.slim.min.js`
- Sizzle `sizzle.js` or `sizzle.min.js`. More info at http://sizzlejs.com.

### Foundation

Minimum requirements for usage are `js/foundation/foundation.core.js`, `js/foundation/foundation.util.mediaQuery.js` and `js/app.js` files.
Find requirements of each Foundation's feature in [the documentation](http://foundation.zurb.com/sites/docs/) and add needed files manually or with the loader.

## Motion-ui

A Sass library for creating CSS transitions and animations from your friends at [ZURB](http://zurb.com). Originally integrated into [Foundation for Apps](http://foundation.zurb.com/apps), the code is now a standalone library and can be used by [Foundation for Sites](http://foundation.zurb.com/sites) and Foundation for Apps.

### Usage

In `scss/app.scss` file uncomment lines below to enable:
```
@import 'motion-ui/motion-ui';

@include motion-ui-transitions;
@include motion-ui-animations;
```
Or use `scss/motion-ui.scss` as a standalone plugin.

Include js-file:
```html
<script src="js/motion-ui/motion-ui.js"></script>
```

## What-input

A global utility for tracking the current input method (mouse, keyboard or touch).

Read [What-input documentation](https://github.com/ten1seven/what-input).

### Usage

```html
<script src="assets/scripts/what-input.js"></script>
```

