# Pre Rating
Pre-Rating is a composition that offers rating with [font-awesome](http://fontawesome.io/)
 icons.

[![NPM](https://nodei.co/npm/pre-rating.png)](https://nodei.co/npm/pre-rating/)

[![npm version](https://badge.fury.io/js/pre-rating.svg)](https://badge.fury.io/js/pre-rating)

## Installation

```
npm install --save pre-rating
```
## For More Example
[Live Demo](https://presort.github.io/pre-rating/)

## Basic Usages

```js

 <Rating currentValue={8}
         onChange={this.__handleChange}
         onMouseOver={this.__handleMouseOver}
 />
```

```js

 <Rating size={2}
  currentValue={4.5}
  onChange={this.__handleChange}
  disabled
 />
```

--- With another font-awesome icons ---

```js

  <Rating size={1}
          iconCount={5}
          initialIcon="fa-heart-o"
          selectedIcon="fa-heart"
          style={{color: "red"}}
          onChange={this.__handleChange}
   />

```

--- Functions return event ----

```js
__handleMouseOver(e) {
    console.log(e.target.value, e.target.parsedValue);
}

__handleChange(e) {
    console.log(e.target.value, e.target.parsedValue);
};

```

## Rating Props

| Name | Type | Default | Required | Description |
|------|------|---------|----------|------------ |
| size | number | 0 | false |Size of Rating icons. Possible Values : 0,1,2,3,4|
| currentValue | number | - | false |Direct selected value.|
| iconCount | number | 10  |false |Count of icons.|
| initialIcon | string | fa-star-o | false |Initial icon type (Works with font-awesome icons like "fa-star-o").|
| selectedIcon | string | fa-star | false |Selected icon type (Works with font-awesome icons like "fa-star").|
| disabled | bool | false | false |Disable icons.|
| onChange | func | - | false |Change event for the component (Returns (clickedKey)).|
| onMouseOver | func | - | false |MouseOver event for the component (Returns (hoveredKey)).|
| style | object | - | false |Style of Rating icons.|
| label | string | - | false |Label for Rating component.|


### Quick Start

#### 1. Get the latest version
You can start by cloning the latest version of pre-rating.

#### 2. Run `npm install`
This will install both run-time project dependencies and developer tools listed
in [package.json](./package.json) file.

#### 3. How to start project in Development Mode

This will start the development server and serve site application.

```shell
$ npm start
```
  
Open Browser and enter `http://localhost:3000` (default) 

### How to Build for Production

If you need just to build the app (without running a dev server), simply run:

```shell
$ npm run build
```

### How to Build for Site

If you need just to build the app (without running a dev server), simply run:

```shell
$ npm run site
```

## License

The MIT License (MIT) Copyright (c) 2017 Fatih Totrakanlı