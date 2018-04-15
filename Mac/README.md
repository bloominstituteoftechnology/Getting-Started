# Welcome to Lambda School's Installation Guide for macOS
- suggestion: Keep apps to Dock.

# Development Environment Set-Up
1. Open the Safari web browser.
2. Install the Google [Chrome](https://www.google.com/chrome/) web browser.
3. Close Safari.
4. Open Chrome.
5. Download [Git](https://git-scm.com/download/mac) tools.
  - Confirm your installation. The version check command should report similarly:
  ```console
  $  git version
         git version 2.15.1 (Apple Git-101)
  ```
6. Install the LTS (Long Term Support - i.e. "stable") version of [NodeJS](https://nodejs.org/).
  - Confirm your installation:
  ```console
  $  node -v
         v8.11.1
  $  npm -v
         5.6.0
    ```
7. Install a Text Editor:
  - [Atom](https://atom.io/)
  - [Visual Studio Code](https://code.visualstudio.com/download)
  - [Sublime](https://www.sublimetext.com/3) (nagware)
  - [Brackets](http://brackets.io/)
8. Install Xcode and the Xcode CLI (Command Line Interface) tools:
  - Install Xcode: https://developer.apple.com/xcode/downloads/
  - Confirm your installation:
  ```console
  $  xcode-select --version
         xcode-select version 2349.
  ```
  - Install Xcode CLI tools: https://developer.apple.com/download/more/
  - Xcode CLI installs additional tools such as `gcc`. Confirm your installation by using the `version` command on one to the tools Xcode CLI installs. You should see something like this:
  ```console
  $  gcc --version
         Configured with: --prefix=/Applications/Xcode.app/Contents/Developer/usr --with-gxx-include-dir=/Applications/Xcode.app/Contents/Developer/Platforms/MacOSX.platform/Developer/SDKs/MacOSX10.13.sdk/usr/include/c++/4.2.1
         Apple LLVM version 9.1.0 (clang-902.0.39.1)
         Target: x86_64-apple-darwin17.5.0
         Thread model: posix
         InstalledDir: /Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin
  ```
  - If you see the following, then you have not yet installed Xcode CLI tools:
  ```bash
  $ gcc
      xcode-select: note: no developer tools were found at '/Applications/Xcode.app', requesting install. Choose an option in the dialog to download the command line developer tools.
  ```
  - NOTE: there are also the Additional Tools for Xcode, but I don't think we need these for Lambda School:
  > This package includes audio, graphics, hardware i/o and auxiliary tools formally bundled in Xcode. These tools include: AU Lab, HALLab, OpenGL Driver Monitor, OpenGL Profiler, Pixie, Quartz Composer, Quartz Composer Visualizer, Quartz Debug, Apple Bluetooth Guidelines Validation (Requires macOS Sierra), Bluetooth Explorer (Requires macOS Sierra), HomeKit Accessory Simulator, IO Registry Explorer, Network Link Conditioner.prefpane, PacketLogger, Printer Simulator,  64BitConversion, Clipboard Viewer, CrashReporterPrefs, Dictionary Development Kit, Help Indexer, Modem Scripts and Repeat After Me.

9. Install [Zoom](https://zoom.us/download).
10. Install [Slack](https://slack.com/downloads/osx).
11. Install [MongoDB Community Edition](https://www.mongodb.com/download-center?jmp=nav#community)
  - https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/
  - Choose the Current Stable Release (Currently 3.6.3)
  - Select "OS X 10.7+ 64-bit w/SSL x64"
  - Download and install
  - Or, you can [follow the instructions to install with Homebrew](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-os-x/#install-mongodb-community-edition-with-homebrew).
12. Install [Compass](https://www.mongodb.com/download-center?jmp=nav#compass)
  - Select the latest verion of "Community Edition Stable" (currently 1.12.4).
  - Select "OS X 64-bit (10.10+)"
  - Download and install.

# other things?
- [Homebrew](https://brew.sh/)
  - remember to `$  brew missing && brew update && brew cleanup && brew cask cleanup && brew prune && brew upgrade && brew doctor` often. Twice ...or more. The `&&` syntax means if one fails, the others won't run. Maybe this isn't best practice to always be upgrading... maybe don't need cask cleanup? ::thinks:: https://medium.com/@waxzce/keeping-macos-clean-this-is-my-osx-brew-update-cli-command-6c8f12dc1731 & brew cask (doctor cleanup upgrade) https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md
- telnet (no longer a part of macOS): `brew install telnet`
- [PostMan](https://www.getpostman.com)
- [React Native SDK](https://developers.facebook.com/docs/react-native)
- [Expo XDE](https://expo.io/tools#client) (React-Native) - LOOK FOR NOTE on how to get Expo to reload fast
- [ngrok](https://ngrok.com/download) Also available through `npm install ngrok` & `brew install ngrok`
- [Firefox](https://www.mozilla.org/en-US/firefox/new/) & [Opera](https://www.opera.com/)? Opera has "free" VPN :\
- [ScreenFlow](https://www.telestream.net/screenflow/overview.htm)
- [RoboMongo](https://robomongo.org/download): Robo 3T
- similar type app for mysql? (workbench?) https://dev.mysql.com/downloads/workbench/ (Confirm the set up)

# Join the club!
- [ ] [Zoom](https://www.zoom.us/signup)
- [ ] [Slack](https://slack.com/)
- [ ] [GitHub](https://www.github.com/)
- [ ] [Google](https://accounts.google.com/SignUp)
- [ ] [Piazza](https://piazza.com/signup)
- [ ] [Repl.it](https://repl.it/signup)
- [ ] [CodePen](https://codepen.io/)
- [ ] [Trello](https://trello.com/signup)
- [ ] [LinkedIn](https://www.linkedin.com)
- [ ] [MLab](https://mlab.com/signup/)

# Speedy macOS tricks
- `⌘ + spacebar` for the Spotlight Search.
- `⌘ + tab` to cycle through applications.
- macOS: check out the Digital Color Meter app (In the /Applications/Utilities folder)
- `cmd + SHIFT + 3` Screen grab
- `cmd + SHIFT + 4` Select area screen grab
- https://gist.github.com/dergachev/4627207
- https://gifox.io/function
- Is everything up to date?
  ```console
  $  softwareupdate --list
      Software Update Tool

      Finding available software
      No new software available.
  ```

# Chrome magic
- React Developer Tools plugin. not sure about this url: https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi
- Redux Developer Tools plugin or this one: https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd
- [One Tab](https://www.one-tab.com/) plug-in to minimize open tabs into a list of URLs
- [HTTPS Everywhere](https://www.eff.org/https-everywhere) (& [Ad Blocker](https://www.eff.org/privacybadger)? From EFF).
- `⌘ + l` focuses to the Location Bar.
- `cmd+option+ left or right arrow` to cycle through open tabs

# Text Editor efficiency
- Global project search: ctrl-shift-f VSC, cmd+shift+f Atom
- Select matching pattern: cmd/ctrl+D Atom/VSC

# Command Line Interface Tools Installed with Xcode CLI
- As far as I know, you do not _need_ the XCode.app, just the CLI Tools.
- In particular, you will be using `gcc` and `make`.
- With their installation, you will receive a host of developer tools:
```
ar
as
asa
bison
BuildStrings
c++
c89
c99
cc
clang
clang++
cmpdylib
codesign_allocate
CpMac
cpp
ctags
ctf_insert
DeRez
dsymutil
dwarfdump
dyldinfo
flex
flex++
g++
gatherheaderdoc
gcc
gcov
GetFileInfo
git
git-cvsserver
git-receive-pack
git-shell
git-upload-archive
git-upload-pack
gm4
gnumake
gperf
hdxml2manxml
headerdoc2html
indent
install_name_tool
ld
lex
libtool
lipo
lldb
lorder
m4
make
MergePef
mig
mkdep
MvMac
nasm
ndisasm
nm
nmedit
otool
pagestuff
projectInfo
ranlib
rebase
redo_prebinding
ResMerger
resolveLinks
Rez
RezDet
RezWack
rpcgen
segedit
SetFile
size
SplitForks
strings
strip
svn
svnadmin
svndumpfilter
svnlook
svnrdump
svnserve
svnsync
svnversion
unifdef
unifdefall
UnRezWack
unwinddump
what
xml2man
yacc
```
