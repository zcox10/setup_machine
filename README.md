# Overview
Run these commands in a terminal window from start to end in order to set up a data science environment in your machine.  The initial download for Homebrew, iTerm2, zsh, oh-my-zsh are all influenced from this [blog post](https://medium.com/ayuth/iterm2-zsh-oh-my-zsh-the-most-power-full-of-terminal-on-macos-bdb2823fb04c).

# Install Homebrew
Homebrew will act as the main software package system for us to install new packages/environments.

`/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)`

# Install iTerm2
iTerm2 is a great terminal emulator that allows us to have more functionality than a regular terminal window.

`brew cask install iterm2`

# Install zsh
The Z shell is a Unix shell that can be used as an interactive login shell and as a command interpreter for shell scripting. This is simply just a well-designed terminal shell that allows us to use many useful features when scripting.

`brew install zsh`

# Install oh-my-zsh
Oh-My-Zsh is an open source, community-driven framework for managing your ZSH configuration. It comes bundled with a ton of helpful functions, helpers, plugins, themes, etc.

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

When prompted with the question: 
`Do you want to change your default shell to zsh? [Y/n]`
Type: `Y`

# (Optional) Decorate iTerm2 With Material Design Colors
If so desired, you can run these commands in order to customize the layout of your new iTerm2 terminal.  

  1. Open terminal and paste.
  
```
cd Downloads
curl -O https://raw.githubusercontent.com/MartinSeeler/iterm2-material-design/master/material-design-colors.itermcolors
```
  
  2. Open iTerm2 that we already downloaded at the first section
  3. Go to iTerm2 > Preferences > Profiles > Colors Tab
  4. Click Color Presets… at the bottom right
  5. Click Import…
  6. Select the material-design-colors.itermcolors file
  7. Select the material-design-colors from Load Presets…

# Install Docker
Next, we need to install Docker. The technical description is below.  But, essentially, Docker allows us to build "containers" that allows us to install various software packages for development (Python packages, R packages, or any packages that you use daily when developing) that can be utilized regardless of what software packages are previously installed on our local machine.  This concept/tool allow us to reproduce our work on any MacOS machine and make it very easy to pass work from one colleague to another.  

### Technical:
Docker is a set of platform-as-a-service products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels.

`brew install docker`

Test Docker is working 
