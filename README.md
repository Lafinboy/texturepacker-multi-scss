Multiple SCSS spritesheet exporter for TexturePacker
========================

This exporter was created for [TexturePacker](http://www.texturepacker.com/) to enable multiple, unique named sprite sheets and matching style files to be generated.

## Installation ##

1. Locate the TexturePacker **exporters** directory within your filesystem, e.g.

    `C:\Program Files (x86)\CodeAndWeb\TexturePacker\bin\exporters`

1. Clone the multi-scss custom exporter into your Texturepacker exporters folder

    `git clone git@github.com:Lafinboy/texturepacker-multi-scss.git multi-scss`

1. Restart TexturePacker

## Use ##

1. Open TexturePacker and create a new spritesheet.
1. Select Multi-SCSS from the Data Format dropdown.
1. Give the Data File and Texture File matching, unique names, e.g. button-sprite.scss, button-sprite.png
1. You can now use the unique name as the base class name, e.g. button-sprite

## Why did you create this exporter? ##

TexturePacker is an awesome piece of software, but it's one *failing* is that the default CSS exporter uses a static base class named "sprite". This prevents use of multiple spritesheets within a site without manually modifying the output CSS.

A quick search for a solution brought me to [texturepacker-multi-css](https://github.com/robert-wallis/texturepacker-multi-css) by Robert Wallis. This package enabled multiple CSS spritesheet files to be generated, but did not handle generation of pseudo classes from filenames. I've submitted a pull request to fix that issue.

With a solid base to work from I cloned and switched to SCSS output to support my current development environment.
