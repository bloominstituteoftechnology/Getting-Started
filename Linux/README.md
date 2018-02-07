# make sure user is set up as administrator?
- suggestion to pin apps to taskbar

# Development Environment Set-Up
<!-- 1. Open the Edge web browser.
2. Download the Google [Chrome](https://www.google.com/chrome/) web browser.
3. Close Edge.
4. Open Chrome.
5. Download [Git Bash](https://git-for-windows.github.io/) (If you are having trouble, [read this](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)). ???? Just Git bash, right, not the tools for PShell/CMD? https://git-scm.com/download/mac see also: http://www.jamessturtevant.com/posts/5-Ways-to-install-git-on-Windows/ ???TrueType on install???? I think git-from-bash-only??? SSL (not native win secure channel lib)???? CRLF/LF options ???? MinTTY ??? No symbolic links (maybe?) ???
6. Download the LTS (Long Term Support - i.e. "stable") version of [Node](https://nodejs.org/).
7. Download Text Editor ([Atom](https://atom.io/), VSC, vim (comes w/git bash iirc), Sublime(nagware), Brackets)
8. Download [Zoom](https://zoom.us/download).
9. Download [Slack](https://www.slack.com/downloads/windows) (How to stop Slack from auto launching????) -->

### "How do I find out if my Linux computer uses 32-bit or 64-bit?"
<!-- 1. Launch the Control Panel
2. Select System
3. Look at the "System Type" -->

# other things?
<!-- - Package manager like [Chocolatey](https://chocolatey.org/)?
- `telnet` (afaik, not a part of win10 release) https://social.technet.microsoft.com/wiki/contents/articles/38433.windows-10-enabling-telnet-client.aspx see also: http://www.sysprobs.com/install-and-enable-telnet-in-windows-8-use-as-telnet-client
- `curl` is asking for the IE engine? https://youtu.be/qlTVMuONazs
- PostMan
- Expo XDE (React-Native)
- `ngrok`
- Firefox & Opera?
- ScreenFlow
- RoboMongo type app for mysql? (workbench?) -->

# Join the club!
<!-- - [Slack](https://slack.com/)
- [GitHub](https://www.github.com/)
- [Google](https://accounts.google.com/SignUp)
- [Piazza](https://piazza.com/signup)
- [Repl.it](https://repl.it/signup)
- [CodePen](https://codepen.io/)
- [LinkedIn](https://www.linkedin.com) -->

# Speedy 'nix tricks
- Digital color meter: https://alternativeto.net/software/digitalcolor-meter/?platform=linux
- GNOME Screenshot and Screencast ships with Ubuntu: https://help.ubuntu.com/stable/ubuntu-help/screen-shot-record.html

# Chrome magic
- React Developer Tools plugin.
- Redux Developer Tools plugin.
- One Tab plug-in to minimize open tabs into a list of URLs
- HTTPS everywhere (Ad Blocker? From EFF.
- `ctrl + l` focuses to the Location Bar.
- ctrl+option+ left right arrow to cycle through open tabs???

# Text Editor efficiency
<!-- - Global project search: ctrl-shift-f VSC, cmd+shift+f Atom???
- Select matching pattern: cmd(macOS)/ctrl(Win)+D Atom/VSC??? -->

<!-- # Integrating Git Bash into Atom & VSC IDE
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
- but I set the Shell Override to: `C:\Program Files\Git\usr\bin\bash.exe` for it to work.
- if neither work, in Git Bash console, ascertain which bash.exe file you are using with this command:
- `$ which bash`
- and use the Windows syntax for the absolute path `which bash` displays, i.e. `C:\path to bash.exe`.
- once you know the path, you can open the parent folder if you want to see the actual bash.exe.
- In Git Bash, enter `open $(dirname $(which bash))`.
- Then you can see the full Windows syntax pathname in the Windows Explorer bar. -->
