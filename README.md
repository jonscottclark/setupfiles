# @jonscottclark's setup files

Resources to help set up a new Mac environment, or to enhance your current working setup.

---

### OSX Settings

The included `.osx` file is a modified and greatly truncated version of the same file [originally](https://github.com/mathiasbynens/dotfiles/blob/master/.osx) authored by [@mathiasbynens](https://github.com/mathiasbynens); I removed a lot of settings that I thought were unnecessary (or that I honestly didn't understand).

Simply execute the file to apply the new defaults (do this first!):

`$ ./.osx`

(Some settings are app-specific to Google Chrome and iTerm, so ensure you have these installed already, either through Cask or by manually installing them.)

---

#### Homebrew

Install via the [instructions on the homepage](http://brew.sh)

Install a bunch of great formulae via the provided shell script (including [Cask](http://caskroom.io/), which allows you to manage third-party binaries through Homebrew):

`$ ./brew.sh`

---

### iTerm

Download via Cask:

`$ brew cask install iterm2`

Check out the [`iterm`](https://github.com/jonscottclark/setupfiles/tree/master/iterm/) directory for a colour scheme.

I've removed the custom preferences as they were too subject to change, they can contain personal data (paths, etc.) and they are outside the scope of this repo.

To import the colour scheme, type the following while you're in iTerm:

`$ open PastelModified.itermcolors`

You'll need to select the colour scheme from the *Profiles* pane in the iTerm preferences; in the *Colors* tab, choosing Pastel Modified in the *Load Presets...* dropdown.

---

### Development tools

#### n (Node version management)

Install via the latest [instructions at the repository readme](https://github.com/tj/n)

Then install & use a stable version of [Node](https://nodejs.org):

`$ n stable`

##### Node.js modules

Install some global Node.js modules via the provided shell script:

`$ ./npm.sh`

#### rvm (Ruby Version Manager)

Install rvm and a stable version of Ruby via the following commands (from the rvm [homepage](https://rvm.io)):

##### Ruby Gems

Install a few useful gems via the provided shell script:

`$ ./gems.sh`

#### Vagrant

You can download Vagrant via its official website or through Cask (recommended):

`$ brew cask install virtualbox vagrant vagrant-manager`

Remember to install a Vagrant Box, such as Ubuntu Server 14.04 LTS:

`$ vagrant box add ubuntu/trusty64`

#### Sublime Text

Download via Cask:

`$ brew tap caskroom/versions`

`$ brew cask install sublime-text-3`

(Of course, you have a license for this, right?)

Check out the [`sublime`](https://github.com/jonscottclark/setupfiles/tree/master/sublime/) directory for a README with more info on packages to install and other setup tasks specific to ST.

---

### Typeface

I've included the [Input font family](http://input.fontbureau.com/), the typeface for coding and for the command line (it's referenced in my Sublime Text and iTerm preferences).

You can also [download it](http://input.fontbureau.com/download/?customize&fontSelection=fourStyleFamily&regular=InputMono-Regular&italic=InputMono-Italic&bold=InputMono-Bold&boldItalic=InputMono-BoldItalic&a=0&g=ss&i=serif&l=serifs_round&zero=slash&asterisk=height&braces=straight&preset=default&line-height=1.2&email=) and customize it to your liking by changing the base styles, character variations, and the default line height. The download link above will pre-fill the customization controls with the settings I selected when I initially downloaded it. After downloading, drop the files into `/Library/Fonts`.

---

### Shell

My shell of choice is [Fish](http://fishshell.com/docs/current/design.html), the **f**riendly **i**nteractive **sh**ell. It's fast, simple to configure, has a nicer scripting syntax, and is actively maintained and improved upon.

Check out my [dotfiles](https://github.com/jonscottclark/dotfiles) which configure the [fish shell](https://github.com/fish-shell/fish-shell).

---

### Licenses

[MIT License](http://jonscottclark.mit-license.org/) © Jon Scott Clark

[MIT License](https://github.com/mathiasbynens/dotfiles/blob/master/LICENSE-MIT.txt) © Mathias Bynens