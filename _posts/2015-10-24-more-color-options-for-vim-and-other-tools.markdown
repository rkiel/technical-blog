---
layout: post
title:  "Color Scheme For VIM And Other Tools"
date:   2015-10-14 22:08:09
tags:
  - vim
---

Been using the same color scheme in your editor and terminal for a long time?
Looking to spruce up your development environment?
Consider installing and using [Solarized: Precision colors for machines and people](http://ethanschoonover.com/solarized).

## What is Solarized?

Solarized has been around since 2011 and was created by [Ethan Schoonover](http://ethanschoonover.com).
On his website, Ethan describes Solarized in the following way:

> Solarized is a sixteen color palette (eight monotones, eight accent colors) designed for use with terminal and gui applications.
It has several unique properties.
I designed this colorscheme with both precise CIELAB lightness relationships and a refined set of hues based on fixed color wheel relationships.
It has been tested extensively in real world use on color calibrated displays (as well as uncalibrated/intentionally miscalibrated displays) and in a variety of lighting conditions.

<div class="visible-md visible-lg" style="float: right; margin: 0 0 15px 15px;">
<a href="https://raw.githubusercontent.com/altercation/solarized/master/img/solarized-vim.png">
<img src="https://raw.githubusercontent.com/altercation/solarized/master/img/solarized-vim.png" width="400px" />
</a>
</div>

<div class="visible-xs visible-sm" style="float: right; margin: 0 0 15px 15px;">
<a class="btn btn-default" href="https://raw.githubusercontent.com/altercation/solarized/master/img/solarized-vim.png">
View Image
</a>
</div>

I'm not a designer but Solarized has some [unique properties](http://ethanschoonover.com/solarized#features) which seem really cool.

* __Selective contrast__ -- "Black text on white from a computer display is akin to reading a book in direct sunlight and tires the eye."
* __Both sides of the force__ -- The same 16 colors are used to support two color schemes: dark and light.
* __16/5 palette modes__ -- "Solarized works as a sixteen color palette for compatibility with common terminal based applications / emulators. In addition, it has been carefully designed to scale down to a variety of five color palettes for use in design work such as web design."
* __Precision, symmetry__ -- "The monotones have symmetric CIELAB lightness differences, so switching from dark to light mode retains the same perceived contrast in brightness between each value. Each mode is equally readable."
* __Fonts__ -- "Solarized has been designed to handle fonts of various weights and retain readability, from the classic Terminus to the beefy Menlo."

<div style="clear: right;"></div>

## So what does it look like?

Fantastic.  The Solarized website has many sample screnshots featuring various languages.

Here's one of those samples featuring Ruby code in dark mode:

<div class="visible-md visible-lg">
<a href="http://ethanschoonover.com/solarized/img/screen-ruby-dark.png">
<img src="http://ethanschoonover.com/solarized/img/screen-ruby-dark.png" />
</a>
</div>

<div class="visible-xs visible-sm text-center" style="margin: 15px 15px 15px 15px;">
<a class="btn btn-default" href="http://ethanschoonover.com/solarized/img/screen-ruby-dark.png">
View Image
</a>
</div>

And here is the corresponding sample of Ruby code in light mode:

<div class="visible-md visible-lg">
<a href="http://ethanschoonover.com/solarized/img/screen-ruby-light.png">
<img src="http://ethanschoonover.com/solarized/img/screen-ruby-light.png" />
</a>

</div>

<div class="visible-xs visible-sm text-center" style="margin: 15px 15px 15px 15px;">
<a class="btn btn-default" href="http://ethanschoonover.com/solarized/img/screen-ruby-light.png">
View Image
</a>
</div>

I think they both look great.

## Where can I use Solarized?

The Solarized website lists support for a number of popular editors, IDEs and terminal emulators.
If you don't find your tool of choice listed, a quick Google search might be all that is needed.
For example, I did not see Sublime listed but I was able to quickly find a [port on GitHub](https://github.com/braver/Solarized).

While I've heard great things about Sublime, I'm still very old school and my editor of choice is VIM.
Let's look at how you would install Solarized for VIM.

## Installing Solarized for VIM

I organize my repositories locally as a mirror of how they are organized on Github.
You can choose any location you want.

{% highlight bash %}
mkdir -p ~/Github/altercation
cd ~/Github/altercation
{% endhighlight %}

Clone the Solarized repository.

{% highlight bash %}
git clone https://github.com/altercation/vim-colors-solarized.git
{% endhighlight %}

Make sure your personal VIM configuration has a `colors` directory.

{% highlight bash %}
mkdir -p ~/.vim/colors
{% endhighlight %}

Copy the `solarized.vim` file into the `colors` directory of your personal VIM configuration.

{% highlight bash %}
cd vim-colors-solarized
cp colors/solarized.vim ~/.vim/colors
{% endhighlight %}

## Setup Solarized for VIM

As mentioned previously, Solarized has both a dark and a light mode.

To initialize VIM on startup to use the dark mode, add the following to your `.vimrc` file.

{% highlight vim %}
syntax enable
set background=dark
colorscheme solarized
{% endhighlight %}

To initialize VIM on startup to use the light mode, add the following to your `.vimrc` file.

{% highlight vim %}
syntax enable
set background=light
colorscheme solarized
{% endhighlight %}

Once you are in VIM, you can toggle back and forth between the two modes.

## Final Thoughts

Solarized is a thoughtfully designed color scheme that is easy to install and use with a wide variety of tools.

For more information, visit the [Solarized: Precision colors for machines and people](http://ethanschoonover.com/solarized) website.

