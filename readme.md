
# Uno for KeystoneJS


Uno for KeystoneJS is a port of the [Uno Ghost Theme](http://github.com/daleanthony/uno.git) originally created by [daleanthony.com](http://daleanthony.com).   The theme features a minimal, responsive design with a cover page, disqus comment integration, foundation icons and various colour options.

This project requires the setup and configuration of [KeystoneJS](http://keystonejs.org) using Handlebars (`HBS`) as the rendering option.  Any problems / issues setting up this theme should be raised on this repo and not on the original repo by Dale Anthony.

For instructions on [usage](docs/usage.md) and [installation](docs/installation.md) view the [documentation](docs/readme.md)

## Demo
There's a demo of the Uno-KeystoneJS theme running on my personal website [morgancraft.com](http://morgancraft.com) or you can view the original Ghost verion on the original designers personal website [daleanthony.com](http://daleanthony.com).


## Features

**Cover page**
The landing page for Uno is a full screen 'cover' featuring your avatar, blog title, mini-bio and cover image.

**Built with SASS, using BEM**
If you know HTML and CSS making modifications to the theme should be super simple.

**Responsive**
Uno looks great on all devices, even those weird phablets that nobody buys.

**Disqus comments**
Disqus integration allows users to comment on your posts.

**Foundation icons**
Uno contains the [Foundation icon font by Zurb](http://zurb.com/playground/foundation-icon-fonts-3) which means you can easily add icons. A full list of available icons can be found on the [Foundation Icon](http://zurb.com/playground/foundation-icon-fonts-3) website.

**No-JS fallback**
While JS is widely used, some themes and websites don't provide fallback for when no JS is available (I'm looking at you [Squarespace](http://blog.squarespace.com/)). If for some weird reason a visitor has JS disabled your blog will still be useable.

**1 theme, 5 colour options**
Uno includes 5 different colour options for you to chose from.

**Future**
KeystoneJS is a CMS and has additional features such as Photo Galleries and Contact Forms with new features being planned.  There are plans to support these additional features in time.  Most likely Contact Forms will be added shortly to the KeystoneJS design.

Also, css/feature parity maintenance will be attempted for Ghost as well.

## FAQs

Uno-KeystoneJS is the first attempt to bridge the HBS Rendering Engine of KeystoneJS to be fully-functional with the Ghost Publishing platform.  Questions or Issues with it should be expressed on this project repo and not on the primary Ghost Uno Theme.

### Ghost Theme FAQ

Some common questions are answered on the [Uno FAQ page](http://daleanthony.com/uno-faq/)

## Contact

The best way to contact me is by [dropping me an email](dale@daleanthony.com) or my messaging me on [Twitter](https://twitter.com/daleanthony)

## Licence

[Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/)


## Development

In order to develop or make changes to the theme you will need to have the sass compiler and bourbon both installed.  If you are running a Ghost environment locally then you should already have these installed as those are required to run Ghost.

To check installation run the following commands from a terminal and you should see the `> cli output` but your version numbers may vary.

** SASS **
```bash

sass -v
> Sass 3.3.4 (Maptastic Maple)
```
If for some reason SASS isn't installed follow the instructions from the [Sass install page](http://sass-lang.com/install)

** Bourbon **
```bash

bourbon help
> Bourbon 3.1.8
```
If Bourbon isn't installed follow the installation instructions on the [Bourbon website](http://bourbon.io)

Once installation is verified we will need to go mount the bourbon mixins into the `scss` folder.

From the project root run `bourbon install` with the correct path
```bash
bourbon install --path assets/scss
> bourbon files installed to assets/scss/bourbon/
```

Now that we have the bourbon mixins inside of the `scss` src folder we can now use the sass cli command to watch the scss files for changes and recompile them.

```bash
sass --watch assets/scss:public/css
>>>> Sass is watching for changes. Press Ctrl-C to stop.
```

** MacOSX Maverick **

Some people may receive this error when trying to run the `sass --watch` command

