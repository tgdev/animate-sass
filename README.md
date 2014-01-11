#Animate.scss
*Sassy just-add-water CSS animation*

`animate-sass` is a Sass version of [https://github.com/daneden](Dan Eden's) [https://daneden.me/animate/](animate.css).

##Features
Animate-sass has a couple of features to try and make the most of what Sass has to offer for more effecient development.

###Helpers

####Mixins
There are a couple of Sass mixins that some of the modules use to generate the necessary compiled css.

####Settings
The settings file allows you to set a range of Sass variables which are used by some of the animation modules.


####Animation Module loading
The settings file also allows you to choose which animation modules you'd like to use - by only choosing the animation modules you need, you're keeping the compiled css at it's leanest!

Eg:
$use-fadeIn: false; // This will not be included

$use-fadeOut: true; // This will be included

Modules are arranged by the following animation types;

- attention-seekers
- bounce-enter
- bounce-exit
- fade-enter
- fade-exit
- flippers
- lightspeed
- rotate-enter
- rotate-exit
- special


####Base

This file is where the base `.animated` css rules are defined as well as a required webkit fix for the `body` tag. 


###Animations

All individual animation modules are kept in their own Sass partial file so they can be found easily. You shouldn't need to edit these but feel free to do so.


##Usage

To use animate.scss in your project, you will need to have Sass installed. [http://sass-lang.com/](Visit the Sass site) to find out how to do this.

Once Sass has been installed, you can download or clone this repo into your project's `css` folder and import `animate.scss` into your main Sass stylesheet.

eg:// inside css/style.scss
````
@import "animate-sass/animate"
````

Choose which modules you want to use in you project via the `helpers/settings` file.

Then in your markup, simply add the class `animated` to an element, along with any of the animation class names.

````
    <div class="animated fadeIn">
    	<p>Watch me fade in!</p>
    </div>
````

That's it! You've got a CSS animated element. Super!


##License

Animate.scss is licensed under the MIT license. [http://opensource.org/licenses/MIT](http://opensource.org/licenses/MIT)


##Questions/Comments

You can follow me / ask questions on twitter: [http://www.twitter.com/tom_gillard](@tom_gillard)


##Learn more

You can check out the original animate.css over at [http://daneden.me/animate.](http://daneden.me/animate).
See working examples as well as how to use with javascript or creating custom css classes


##Changelog

v0.2.0 - Removed css source files and restructured repo for better compatibility with user projects
v0.1.0 - Initial port of animate.css to Sass