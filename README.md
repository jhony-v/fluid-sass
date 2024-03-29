<p align="center">
    <img src="./fluid.png" />
</p>


## What is Fluid-Sass?

Fluid sass in a series of scss mixins and css classes to create fluid and spring based motion animations, just include mixin in your class to create fast and beautiful animations.

There are currently **22** animations available **[official documentation](https://jhony-24.github.io/fluid-sass)**.

## Installation

```console
$ npm install fluid-sass 
$ npm install -D fluid-sass 
```

```console
$ yarn add fluid-sass 
```

## Usage 
This command installs the files you need (css, scss). If you are using in development mode, you can use **npx** prefix before **fluid-sass** command.

```console
$ fluid-sass install <typeFile> --dir=<dir>
```
| options | description | options |
| -- | -- | :--: |
| typeFile | Install a file type css or scss in the project | ( css, scss ) |
| dir | The directory to install |


## How to Integrate
See a sample of how to integrate development code in HTML, CSS, SCSS and for more dynamism in Javascript.

### HTML 
Include your class names personalized.
```html
<!-- page.html -->
<link rel="stylesheet" href="animations.css" />

<header class="fluid-bounce">
    <button class="fluid-shake-vertical" id="btn-sign-in">
        Sign in
    </button>
    <button class="fluid-shake-vertical" id="btn-sign-up">
        Sign up
    </button>
</header>
```

### SASS / SCSS 
Include the class name as a mixin to your custom classes.
```scss
@import "animations";
// page.scss
.header-component {
    @include fluid-bounce();
}
.button-component {
    @include fluid-shake-vertical();
}
```

### Javascript
Include the classNames defined into yout project
```javascript
// main.js
let myButton = document.getElementById('btn-sign-up');
byButton.addEventListener('click' , function (e) {
    e.currentTarget.classList.toggle('fluid-shake-vertical');
});

```

## List of class names and mixins animations
The class names is equal to mixins names
| Class names or Mixins names | Type animation |
| --- | :--: |
| fluid-bounce | bounce |
| fluid-bounce-inset | bounce |
| fluid-bounce-rotate | bounce |
| fluid-bounce-expand-x | bounce |
| fluid-bounce-expand-y | bounce |
| fluid-fade | fade |
| fluid-fade-intermittent | fade |
| fluid-fade-left | fade |
| fluid-fade-right | fade |
| fluid-from-left | slide |
| fluid-from-right | slide |
| fluid-from-top | slide |
| fluid-from-bottom | slide |
| fluid-shake | shake |
| fluid-shake-rotate | shake |
| fluid-shake-vertical | shake |
| fluid-shake-cross | shake |
| fluid-shake-skew-x | shake |
| fluid-shake-skew-y | shake |
| fluid-d3-rotate | 3d |
| fluid-d3-triangle | 3d |


View more animations in the documentation following url [fluid-sass documentation](https://jhony-24.github.io/fluid-sass)
