# Development Environment Set-Up
1. Open the Edge web browser.
2. Download the Google Chrome web browser.
3. Close Edge.
4. Open Chrome.
5. Download Git Bash.
6. Download Node.
7. Download Text Editor (Atom, VSC, vim (comes w/git bash iirc), Sublime(nagware), Brackets)
8. Download Zoom
9. Download the Slack.app


# other things?
- Homebrew
- telnet (no longer a part of macOS)
- PostMan
- Expo XDE (React-Native)
- ngrok
- Firefox & Opera?
- ScreenFlow
- RoboMongo type app for mysql? (workbench?)

# Join the club!
- Slack
- GitHub
- Google
- Piazza
- Repl.it
- CodePen
- LinkedIn

# Speedy Win10 tricks
- Cortana, motherfucker!

# Chrome magic
- React Developer Tools plugin.
- Redux Developer Tools plugin.
- One Tab plug-in to minimize open tabs into a list of URLs
- HTTPS everywhere (Ad Blocker? From EFF.
- `ctrl + l` focuses to the Location Bar.
- ctrl+option+ left right arrow to cycle through open tabs???

# Text Editor efficiency
- Setting up VSC to use Git Bash on Windows
  - https://code.visualstudio.com/docs/editor/integrated-terminal
  - hacky workaround to have both bash and Powershell available in the VSC terminal selector: http://jeffa.tech/vscode-multiple-integrated-terminals/
  ```json
  // Place your settings in this file to overwrite the default settings
  {
      // Git Bash
      "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
      // PowerShell
      "terminal.integrated.shell.windows2": "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
  }
  ```
- Setting up Atom with an integrated console: https://atom.io/packages/platformio-ide-terminal (PShell default)
  - Setting up Atom for Git Bash integrated console: https://forum.freecodecamp.org/t/bash-on-ubuntu-on-windows-on-atom/44948
  - `C:\\Windows\\sysnative\\bash.exe`
- Global project search: ctrl-shift-f VSC, cmd+shift+f Atom???
- Select matching pattern: cmd(macOS)/ctrl(Win)+D Atom/VSC???
