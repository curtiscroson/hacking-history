# Setup

## OSX

To get started with Python for OSX, you need to open your Terminal application. You can find this tool located in the 'Applications' folder, inside the 'Utilities' subdirectory. Double click it to open your command-line terminal.

You should see a small window pop up, with some text readout. On the active line, you should see your user information followed by a '$' symbol (e.g. MacbookPro:~ dave_thomas$) and then a blank cursor. If you type or paste anything into the terminal and then press enter, it will execute the commands.

In what follows below, anything in grey code blocks is to be entered in the terminal (except for lines starting with '#', which are comments). Each '@user $' indicates the start of a new command.

First, you need to install some of Apple's XCode software libraries. Type the following command, and then confirm any dialog boxes that pop up. This may take a minute.
``` shell
# Brings up dialog to download & install XCode
@user $ xcode-select --install
```

Next, we are going to install Homebrew, which is a small and excellent package manager for OSX. This will allow you to install many useful tools without cluttering up your system or dealing with messy configurations.

Copy and paste the torturous looking command into your terminal and Homebrew will download and install.
``` shell
# Issue command to d/l and install OSX's package manager, Homebrew
@user $ /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Now we can use the command `brew` to install any further command-line tools easily. The following comands will install the core tools needed for this class.
``` shell
@user $ brew update
@user $ brew tap caskroom/cask
@user $ brew install npm wget python python3
@user $ brew cask install github sublime-text
@user $ brew cleanup
```

Now you should be able to use the commands `python`, `python3`. In addition, each comes with its own package manager `pip` and `pip3`, which can be used to automatically download and install module packages. You will also find that Github Desktop and Sublime Text 3 have been added to your applications directory.

## Windows