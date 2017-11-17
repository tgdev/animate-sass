# animate-sass

_*Sassy just-add-water CSS animation*_

**animate-sass** is a Sass version of [Dan Eden's](https://github.com/daneden) [Animate.css](https://daneden.me/animate/).

### Installation

Add animate-sass to your project using one of the methods below.

**NPM: [https://www.npmjs.com/](https://www.npmjs.com/)**
```bash
$ npm install animate-sass --save-dev
```

**Yarn: [https://yarnpkg.com/en/](https://yarnpkg.com/en/)**
```bash
$ yarn add animate-sass --dev
```

**Bower: [http://bower.io](http://bower.io)**
```bash
$ bower install animate-sass
```

### Features
**animate-sass** has a couple of features to make the most of what Sass has to offer for more efficient development.

##### Animations

All individual animation modules are kept in their own [Sass partials](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#partials) so they can be found easily. You shouldn't need to edit these as they are part of the animate.css library.

Modules are arranged by the following animation types;

| Animation Types   |
|-------------------|
| attention-seekers |
| bounce-enter      |
| bounce-exit       |
| fade-enter        |
| fade-exit         |
| flippers          |
| lightspeed        |
| rotate-enter      |
| rotate-exit       |
| special           |


##### Helpers

**Base Styles**
The `helpers/_base.scss` file contains the main `.animate` css rules for animate-sass to work.

**Mixins**
There are a couple of [Sass mixins](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#mixins) defined in `helpers/_mixins.scss` that some of the modules use to generate the necessary compiled css.

**Settings**
The `helpers/_settings.scss` file defines a range of default [Sass variables](http://sass-lang.com/documentation/file.SASS_REFERENCE.html#variables_) which are used by some of the animation modules. You can override the defaults in your own settings or style sass file(s).


##### Animation Module loading
The settings file also sets all animation modules to false (nothing gets loaded).
To include an animation module in your project, simply override the `$use-[moduleName]` variable in your own settings file to true.

**By only choosing the animation modules you need, you're keeping the compiled css at it's leanest!**

Eg:
```scss
// These animation modules will be included in output css
$use-fadeIn: true;
$use-fadeOut: true;
```


### Usage

To use `animate.scss` in your project, you will need to have Sass installed. [Visit the Sass site](http://sass-lang.com/) to find out how to do this.

Once Sass has been installed, you can download or clone this repo into your project and import `animate.scss` into your main Sass stylesheet.

Eg: inside `css/style.scss`
```scss
@import "[path-to-node_modules-or-bower_components]/animate-sass/animate";
```

Choose which modules you want to use in you project by overriding the variables set in the `helpers/_settings.scss` file in your own settings or variables file.

Eg: inside `_vars.scss`
```scss
...
// These override the default vars inside animate-sass/helpers/_settings.scss
$use-fadeIn: true;
$use-fadeOut: true;
...
```

Eg: inside `css/style.scss`
```scss
@import "vars"; // project's Sass vars file
@import "[path-to-node_modules-or-bower_components]/animate-sass/animate";
```

Finally in your markup, simply add the class `animated` to an element, along with any of the animation class names.

**You may also want to include the class infinite for an infinite loop.**

```html
    <div class="animated fadeIn">
    	<p>Watch me fade in!</p>
    </div>
```

That's it! You've got a CSS animated element. Super!


### License

Animate.scss is licensed under the MIT license. [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)


### Contributing

Pull requests are where it's at!

Apologies in advance for the slow action on pull requests and issues. When submitting your pull request please make sure you match the naming convention (camelCase, categorised [fades, bounces, etc]).


### Learn more

You can [check out Dan Eden's original animate.css here](http://daneden.me/animate). See working examples as well as how to use with javascript or creating custom css classes


### Change log

See [Changelog](CHANGELOG.md)
