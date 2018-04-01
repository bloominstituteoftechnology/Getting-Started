# Welcome to Lambda School's Installation Guide for macOS
- suggestion: add apps to Dock.

#### TODO: Mongo

# Development Environment Set-Up
1. Open the Safari web browser.
2. Download the Google [Chrome](https://www.google.com/chrome/) web browser.
3. Close Safari.
4. Open Chrome.
5. Download [Git](https://git-scm.com/download/mac) tools.
6. Download the LTS (Long Term Support - i.e. "stable") version of [Node](https://nodejs.org/).
7. Download a Text Editor:
  - [Atom](https://atom.io/)
  - [Visual Studio Code](https://code.visualstudio.com/download)
  - [Sublime](https://www.sublimetext.com/3) (nagware)
  - [Brackets](http://brackets.io/)
8. Install Xcode CLI (Command Line Interface): tools <<< may not be necessary?
  - Install Xcode: https://developer.apple.com/xcode/downloads/
  - Install Xcode CLI tools: https://developer.apple.com/download/more/
9. Download [Zoom](https://zoom.us/download).
10. Download [Slack](https://slack.com/downloads/osx).

# other things?
- [Homebrew](https://brew.sh/)
  - remember to `$  brew missing && brew update && brew cleanup && brew cask cleanup && brew prune && brew upgrade && brew doctor` often. Twice ...or more. The `&&` syntax means if one fails, the others won't run. Maybe this isn't best practice to always be upgrading... maybe don't need cask cleanup? ::thinks:: https://medium.com/@waxzce/keeping-macos-clean-this-is-my-osx-brew-update-cli-command-6c8f12dc1731 & brew cask (doctor cleanup upgrade) https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md
- telnet (no longer a part of macOS): `brew install telnet`
- [PostMan](https://www.getpostman.com
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
