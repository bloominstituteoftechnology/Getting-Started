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
- Global project search: ctrl-shift-f VSC, cmd+shift+f Atom???
- Select matching pattern: cmd(macOS)/ctrl(Win)+D Atom/VSC???

# Integrating Git Bash into Atom & VSC IDE
### VSC
- Setting up VSC to use Git Bash on Windows
- https://code.visualstudio.com/docs/editor/integrated-terminal
NOTE: maybe overkill to set it up with both? maybe worth documenting and hiding?

<details><summary>Expand if you want BOTH bash and PowerShell available in VSC</summary><p>

- hacky workaround to have both bash and Powershell available in the VSC terminal selector: http://jeffa.tech/vscode-multiple-integrated-terminals/
1. `ctrl + comma` will load your user settings in VSC
2. Modify your User Settings:
```js
// Place your settings in this file to overwrite the default settings
{
    // Git Bash
    "terminal.integrated.shell.windows": "C:\\Program Files\\Git\\bin\\bash.exe",
    // PowerShell
    "terminal.integrated.shell.windows2": "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
}
```

3. ``ctrl + tilda/backtick (~/`)`` to open editor. It should say `1. bash`
4. add the `2` t the end of the bash key and remove it from the powershell key, like so:
```js
// Place your settings in this file to overwrite the default settings
{
    // Git Bash
    "terminal.integrated.shell.windows2": "C:\\Program Files\\Git\\bin\\bash.exe",
    // PowerShell
    "terminal.integrated.shell.windows": "C:\\Windows\\System32\\WindowsPowerShell\\v1.0\\powershell.exe"
}

```

5. now press the plus sign to create a new terminal. It should say `2. powershell`
6. now swap the `2` back to how it looked in step 2.
7. Now any new consoles you create will be bash, but you'll have a persistent option 1 & 2.

</p></details>

### Atom
- Setting up Atom with an integrated console: https://atom.io/packages/platformio-ide-terminal (PowerShell is the default)
1. `ctrl + ,` for settings
2. select `+ Install`
3. 3. type in `platformio-ide-terminal`
4. Install the platformio-ide-terminal package!
5. ``ctrl + tilda/backtick (~/`)`` to launch a new terminal in Atom.
6. `alt + shift + t` to make a new console
7. `alt + shift + j/k` to cycle through them

- Setting up Atom for an integrated console using your Git Bash: https://forum.freecodecamp.org/t/bash-on-ubuntu-on-windows-on-atom/44948
- NOTE: the article says to set to: `C:\\Windows\\sysnative\\bash.exe`
- but I set to: `C:\Program Files\Git\usr\bin\bash.exe` for it to work.
- if neither work, in Git Bash console, ascertain which bash.exe file you are using with this command:
- `$ which bash`
- and use the Windows syntax for the absolute path `which bash` displays, i.e. `C:\path to bash.exe`.
- once you know the path, you can open the parent folder if you want to see the actual bash.exe.
- In Git Bash, enter `open $(dirname $(which bash))`.
- Then you can see the full Windows syntax pathname in the Windows Explorer bar.
