# @jonscottclark's setup files

Resources to help set up a new Mac environment, or to enhance your current working setup.

## Essential Apps

### Homebrew

Install via the [instructions on the homepage](http://brew.sh)

Install a bunch of great formulae via the provided shell script:

`$ ./brew.sh`

### nvm (Node Version Manager)

Install via the latest [instructions at the repository readme](https://github.com/creationix/nvm#install-script)

Then install a stable version of [Node](https://nodejs.org):

`$ nvm install 0.10`

### rvm (Ruby Version Manager)

Install rvm and a stable version of Ruby via the following commands (from the rvm [homepage](https://rvm.io)):

`$ gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3`

`$ \curl -sSL https://get.rvm.io | bash -s stable --ruby=2.1.1`

### Vagrant

You can download Vagrant via its official website or through Cask (recommended):

`$ brew cask install virtualbox vagrant vagrant-manager`

Remember to install a Vagrant Box, such as Ubuntu Server 14.04 LTS:

`$ vagrant box add ubuntu/trusty64`

### Sublime Text

Download via Cask:

`$ brew tap caskroom/versions`
`$ brew cask install sublime-text-3`

(Of course, you have a license key for this, right?)

Install [Package Control](https://packagecontrol.io/installation) and some [really useful packages](https://github.com/jonscottclark/setupfiles/blob/master/sublime/PACKAGES.md).

Check out the [`sublime`](https://github.com/jonscottclark/setupfiles/tree/master/sublime/) directory for preferences to import.

### iTerm

Download via Cask:

`$ brew cask install iterm2`

Check out the [`iterm`](https://github.com/jonscottclark/setupfiles/tree/master/iterm/) directory for preferences to import and a colour scheme.

To use the colour scheme, type the following while you're in iTerm:

`$ open PastelModified.itermcolors`

## OSX Settings

The included `.osx` file is a modified and greatly truncated version of the same file [originally](https://github.com/mathiasbynens/dotfiles/blob/master/.osx) authored by @mathiasbynens; I removed a lot of settings that I thought were unnecessary (or that I honestly didn't understand).

Simply execute the file to apply the new defaults:

`$ ./.osx`

(Some settings are app-specific to Google Chrome and iTerm, so ensure you have these installed already, either through Cask or by manually installing them.)

## Typeface

I've included the [Input font family](http://input.fontbureau.com/), the typeface for coding and for the command line (it's referenced in my Sublime Text and iTerm preferences).

You can also [download it](http://input.fontbureau.com/download/?customize&fontSelection=fourStyleFamily&regular=InputMono-Regular&italic=InputMono-Italic&bold=InputMono-Bold&boldItalic=InputMono-BoldItalic&a=0&g=ss&i=serif&l=serifs_round&zero=slash&asterisk=height&braces=straight&preset=default&line-height=1.2&email=) and customize it to your liking by changing the base styles, character variations, and the default line height. The download link above will pre-fill the customization controls with the settings I selected when I initially downloaded it.

## Shell

I maintain a [personal dotfiles repo](https://github.com/jonscottclark/dotfiles) which contains configuration for zsh, head over there for shell goodies.