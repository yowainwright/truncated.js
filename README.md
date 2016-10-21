[![npm version 0.1.1](https://badge.fury.io/js/truncated.js.svg)](https://www.npmjs.com/package/truncated.js)
[![Bower version 0.1.1](https://badge.fury.io/bo/truncated.js.svg)](https://github.com/yowainwright/truncated.js)

# Truncated.js

> A plugin for effeciently and semantically truncating text.

This project will is now called **shave** and will better be supported [here](https://github.com/dollarshaveclub/shave).

## Setup

```terminal
npm i truncated.js --save-dev
```
or
```terminal
bower i truncated.js --save-dev
```

## Run

1. Add **dist/truncated.js**.
2. `truncate` text within the element you'd like to.

```javascript
truncated('selector', maxHeight);🔥
```

## Basic Examples

**Basic**
```javascript
truncated('selector', maxHeight);
```

**Or Multiples**
```javascript
truncated('selector', maxHeight);
```

**But not this one**
```javascript
truncated('selector:not([not this selector])', maxHeight);
```
**With a special symbol**
```javascript
truncated('selector', maxHeight, {character:'🍻'});
```

**With a special CSS Class**
```javascript
truncated('selector', maxHeight, {character:'🙌', classname:'your-css-class'});
```

**Or with jQuery**
```javascript
$('selector').truncated(maxHeight);
```

## How?

**Truncated.js** trims an element's text string to the last full word that can fit within a specified max height.

## Why?

**Truncated.js** is made for simpicity; it doesn't try to oversolve truncation or provide tons of options. It truncates text to a max height.

## What about the original text?

**Truncated.js** re-adds the _diff_ of the original seleected elements's text in a hidden `<span>`. It runs a check for that `<span>` to make sure text is truncated as desired every time.

## What about size?

**Truncated.js** is small - `~1.5kb` unminified and is meant to do 1 thing - _truncate text to fit beatifully to a specified max height_.

## How can I use it?

You can use **Truncated.js** in all modern formats and as a `jQuery` or `zepto` plugin.
