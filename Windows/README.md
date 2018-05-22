# Welcome to Lambda School's Installation Guide for your Windows operating system
- suggestion: pin apps to taskbar, also include snipping tool for screen grabs.

### "How do I find out if my Windows computer uses 32-bit or 64-bit?"
1. Launch the Control Panel
2. Select System & Security
3. Select System
4. Look at the "System Type"

Or, try these commands in CMD or Powershell:
```console
> wmic os get caption
> wmic os get osarchitecture
```

# Development Environment Set-Up
1. Open the Edge web browser.
2. Install the Google [Chrome](https://www.google.com/chrome/) web browser.
3. Close Edge.
4. Open Chrome.
5. Install [Git Bash](https://git-for-windows.github.io/). Also available here: https://git-scm.com/download/win (If you are having trouble, [read this](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)).
    * Just GitBash or the tools for PShell/CMD? See also: http://www.jamessturtevant.com/posts/5-Ways-to-install-git-on-Windows/
    * With Git installer: TrueType on install? I think git-from-bash-only or CMD too? SSL (not native win secure channel lib)? CRLF/LF options (suggested)? MinTTY? No symbolic links (maybe)? SEE PICS.
6. Install the LTS (Long Term Support - i.e. "stable") version of [NodeJS](https://nodejs.org/).
7. Install [Yarn](https://yarnpkg.com). Options:
    1. Yarn Installer: https://yarnpkg.com/latest.msi
    2. If you are already very comfortable and confident with the package manager, "Chocolatey" you can install Yarn with the [Chocolatey](https://chocolatey.org/) package manager. Follow [these instructions](https://chocolatey.org/install).
    ```console
    choco install yarn
    ```
8. Install a Text Editor ([Atom](https://atom.io/), [VSC](https://code.visualstudio.com/download), vim (comes w/git bash iirc), Sublime(nagware), Brackets, et cetera.)
9. Install [PostMan](https://www.getpostman.com).
10. Install [MongoDB Community Server](https://www.mongodb.com/download-center?jmp=nav#community)
  - Select the "Community Server" tab
  - Select Windows for the Current Stable Release (Currently 3.6.4)
  - Version: "Windows Server 2008 R2 64-bit and later, with SSL support x64"
  - Download the installation package (msi) and install
  - > During the installation process you will be given the option to install MongoDB Compass in addition to MongoDB Server.
  - **WARNING: DO NOT INCLUDE COMPASS WITH MONGODB INSTALL**: https://youtu.be/l8Ij6hVQsBk
  - In CMD, create a data directory: `>md \data\db`
      - Confirm the directory has been made with `>dir \data`
  - ALSO NOTE: After the install, the `mongo` and `mongod` commands should work in GitBash BUT there are issues with MinTTY allowing ctrl-c to kill the mongod process. See here: https://github.com/nodejs/node/issues/16103 You can use the `netstat` command to find out which process ID the mongo daemon is running on, and then from CMD or PowerShell use the `Taskkill` command to end the process:
  ```
  >netstat -aon
  >Taskkill /PID {PID number} /F
  ```

  - Add `C:\Program Files\MongoDB\Server\3.6\bin\` directory to PATH environmental variable for easy command line interaction:
    1. Get the location of the executable: `C:\Program Files\C:\Program Files\MongoDB\Server\3.6\bin`
    2. You can also get this from the executable file by right-clicking on the "mongo" and "mongod" files and selecting "Properties".
    3. Run the command `SystemPropertiesAdvanced` in CMD
    4. Click "Environment Variables"
    5. Select the "Path" item (top half for the user variables)
    6. Select "Edit"
    7. Select "New"
    8. Paste in the new environmental variable path: `C:\Program Files\MongoDB\Server\3.6\bin`
    9. Select OK and exit the Advanced System Properties. Now you can run mongo and mongod in CMD and PowerShell.
  - Detailed installation guide: https://docs.mongodb.com/manual/tutorial/install-mongodb-on-windows/
11. Install [Compass](https://www.mongodb.com/download-center?jmp=nav#compass) separately
  - Select the latest verion of "Community Edition Stable" (currently 1.12.5).
  - Select "Windows 64-bit (7+)"
  - Download and install - it will install automatically.
  - https://docs.mongodb.com/compass/master/
12. Install [Zoom](https://zoom.us/download).
  - You may also want the plugin for Outlook or the Extension for the Chrome browser (scroll down on the Downloads page).
13. If you haven't already, install [Slack](https://www.slack.com/downloads/windows)
  - You can disable Slack from automatically starting up through the Task Manager

# other things?
- Package manager? Use MSI (MicroSoft Installer). Only use package managers like [Chocolatey](https://chocolatey.org/) if you are already VERY comfortable with them.
- `telnet` (afaik, not a part of win10 release) https://social.technet.microsoft.com/wiki/contents/articles/38433.windows-10-enabling-telnet-client.aspx see also: http://www.sysprobs.com/install-and-enable-telnet-in-windows-8-use-as-telnet-client
- `curl` is asking for the IE engine? https://youtu.be/qlTVMuONazs. Seems to be part of GitBash.
- [React Native SDK](https://developers.facebook.com/docs/react-native)
- [Expo XDE](https://expo.io/tools#client) (React-Native) - LOOK FOR NOTE on how to get Expo to reload fast
- [ngrok](https://ngrok.com/download) Also available through `npm install ngrok` & `brew install ngrok`
- [Firefox](https://www.mozilla.org/en-US/firefox/new/) & [Opera](https://www.opera.com/)? Opera has "free" VPN :\
- [ScreenFlow](https://www.telestream.net/screenflow/overview.htm)
- RoboMongo type app for mysql? (workbench?)

# Speedy Win10 tricks
- Cortana?
  - Maybe you love it.
  - If you don't, reclaim that task bar real estate and give your processor a break: https://www.pcworld.com/article/2949759/windows/killing-cortana-how-to-disable-windows-10s-info-hungry-digital-assistant.html
- Digital color meter: https://graphicdesign.stackexchange.com/q/76383
- the CMD equivalent for `which` is `where`. In Powershell, `where` is an alias for `Where-Object` but you can access the “where” command in PS with `where.exe` or you can use `get-command` in Powershell.
- Powershell: use the `ii` command to open `i`nvoke `i`tem, e.g. `> ii .` will open the current directory in the Explorer.

# Chrome magic
- React Developer Tools plugin: https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en
- Redux Developer Tools plugin: https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en
- One Tab plug-in to minimize open tabs into a list of URLs: https://www.one-tab.com/the CMD equivalent for `which` is `where` and in Powershell, `where` is an alias for `Where-Object` but you can access the “where” command in PS with `where.exe` or you can use `get-command`
- HTTPS everywhere from EFF: https://www.eff.org/https-everywhere
- Privacy Badger from EFF: https://www.eff.org/privacybadger
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

- Set the Shell Override to: `C:\Program Files\Git\usr\bin\bash.exe` for it to work.
- if this doesn't work, in the Git Bash console, ascertain which bash.exe file you are using with this command:
- `$ which bash`
- and use the Windows syntax for the absolute path `which bash` displays, i.e. `C:\path to bash.exe`.
