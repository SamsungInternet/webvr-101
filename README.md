# WebVR: Getting Started with Virtual Reality on the Web (SDC 2017)

**Welcome! This is a short tutorial created especially for the Samsung Developer Conference 2017. Within a few minutes, you should have your own Virtual Reality web application that you can try out in a Samsung Gear VR headset!**

We are using the excellent, open source [A-Frame](https://aframe.io/) library which makes creating WebVR applications much easier. You can create fantastic scenes just by writing HTML! There are many components available that make it easy to add objects, lighting, interactivity and more.

## Instructions

If you have any difficulties or questions at any point, just let us know and we can lend a hand!

### Getting Started

1. Click 'Remix this' to make your own version of this project.

1. Click 'Show Live' to see how it looks already. You should some text and a box. 

1. You can move around the scene with your mouse, keyboard (WASD keys) or trackpad.

1. To try this out in the Gear VR headset, you will need a Samsung phone. You can borrow one from us if you don't have one. Open up the Samsung Internet browser (labelled "Internet").

1. Take a look at the URL for your project. Type in this URL in the Samsung Internet URL bar.

1. Now put the smartphone in a Gear VR headset. Once you put the headset on, you should see the same scene inside a window in Virtual Reality! 

1. Tap on the trackpad on the side of the headset to 'click' on the goggles icon in the bottom-right corner. This will make the scene fill the whole 360 degree environment!

1. (Back in the real world!) Open up `index.html` and take a look at the code. You should see the `<a-text>` and `<a-box>` elements that make those objects appear in the scene.

1. If you like, you can try changing their properties and see what effect this has. The `color` is a hex value like in CSS. The `position` contains three values for the `x`, `y` and `z` axes.

### Building Your Scene

1. Our virtual world is a bit grey at the moment! Let's add a 'skybox' to give ourselves a proper environment. Replace the current `<a-sky>` element with the version that's commented out underneath. You should now be in a more peaceful environment! Feel free to try out other 360 photos too. You can find some in the `assets` directory.

1. Let's make our box spin! Uncomment the `<a-animation>` line inside the `<a-box>` element. You should see the box rotate back and forth.

1. It's time to add a 3D model to the scene. A duck would go nicely on that river! Uncomment the `<a-entity>` with ID 'duck'.

1. Next we are going to introduce a custom 'component'. Components can be added to elements, to introduce customisation and interaction. The component we are going to introduce will let us change the color of objects when we look at them. Uncomment the section that begins with `AFRAME.registerComponent` up in the `<script>` at the top of the page.

1. Finally, let's use this component with our `<a-box>` element. Add `change-color-on-hover="color: yellow"` as an attribute after `<a-box`, before the closing `>` tag. You can change the color to any you like (but yellow should go nicely with the duck!) Now any time you are looking directly at the box, it should change color. When you look away, it should change back again.

You have now created a Virtual Reality scene, with a custom model, animation and interactivity!

### What's Next?

We hope you will go on from here and create amazing virtual worlds! Just bookmark this URL and you can access everything from here: 

[glitch.com/~webvr-101](https://glitch.com/~webvr-101)

Alternatively just let us know and we'll give you a hand-out sheet with the URLs on it.

* The A-Frame documentation contains a wealth of information about the various in-built components and more: [aframe.io/docs/](https://aframe.io/docs/).
* Here are some links to find assets, like 3D models and 360 degree images: [aframe.io/docs/0.6.0/introduction/faq.html#where-can-i-find-assets](https://aframe.io/docs/0.6.0/introduction/faq.html#where-can-i-find-assets).
* Here are some other sample projects we have created: [github.com/samsunginternet/a-frame-demos/](https://github.com/samsunginternet/a-frame-demos/)
