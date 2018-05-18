# Welcome to Lambda School's Installation Guide for your Linux operating system
- You are welcome to use whichever Linux OS you are comfortable with.
- These instructions have been tested with Ubuntu 18.04 LTS.
- These instructions should be applicable to any Debian based Linux system (e.g. Arch, Mint, _et cetera_)
- Suggestion: pin apps to taskbar (Ubuntu equivalent name?)

### "How do I find out if my Linux computer uses 32-bit or 64-bit?"
1. Open the System Settings (from the top right pulldown menu)
2. Click on Details, or
```console
$ lscpu
  Architecture:        x86_64          <--- The "64" means you use 64-bit and it's capable of running both.
  CPU op-mode(s):      32-bit, 64-bit  <--- If you only see the 32-bit mode listed, you’re running a 32-bit version of Linux.
  Byte Order:          Little Endian
  ...
```

# Development Environment Set-Up
1. Open the FireFox web browser.
2. Install the Google [Chrome](https://www.google.com/chrome/) web browser.
3. Close Firefox.
4. Open Chrome.
5. Install [Git](https://git-scm.com/download/linux)
  ```console
  $ sudo apt install git
    ...
  $ git version
    git version 2.17.0
  ```
6. Install the LTS (Long Term Support - i.e. "stable") version of [Node](https://nodejs.org/)
  ```console
  $ sudo apt install nodejs
  $ node -v
    v8.10.0
  ```
7. Install Text Editor ([Atom](https://atom.io/), [Visual Studio Code](https://code.visualstudio.com/download), Sublime, Brackets, et cetera.
8. Install [cURL to install Yarn](https://yarnpkg.com/lang/en/docs/install/#debian-stable)
  ```consoles
  $ sudo apt install curl
  $ curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
    OK
  $ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
    deb https://dl.yarnpkg.com/debian/ stable main
  $ yarn -v
    1.6.0
  ```
9. Install [Postman](https://www.getpostman.com/)
  - Extract Postman from the compressed file, e.g. Postman-linux-x64-6.0.10.tar.gz
  - Move the extracted Postman folder from the Downloads folder to the /opt directory
  ```console
  $ sudo mv ~/Downloads/Postman  /opt/Postman
  ```
  - Create a symbolic link from the application file to your Path
  ```console
  $ sudo ln -s /opt/Postman/Postman /usr/bin/postman
  ```
  - if you get a Gtk-Message: "Failed to load module "canberra-gtk-module" you can `$ sudo apt install libcanberra-gtk-module`
10. Install [MongoDB](https://docs.mongodb.com/manual/administration/install-on-linux/)
  - `$ sudo mkdir -m 777 -p /data/db`
  - Select the latest version of the Community server for Ubuntu from https://www.mongodb.com/download-center?jmp=nav#community
  - Extract MongoDB from the compressed file, e.g. mongodb-linux-x86_64-ubuntu1604-3.6.4.tgz
  - Move the extracted MongoDB folder from the Downloads folder to the /opt Directory
  ```console
  $ sudo mv ~/Downloads/mongodb-linux-x86_64-ubuntu1604-3.6.4 /opt/MongoDB
  $ sudo ln -s /opt/MongoDB/bin/mongod /usr/bin/mongod
  $ sudo ln -s /opt/MongoDB/bin/mongo /usr/bin/mongo
  ```
  - Now both the MongoDB daemon `mongod` and the `mongo` tools are available to you.
11. Install [Compass](https://www.mongodb.com/download-center?jmp=nav#compass)
12. Install [Zoom](https://zoom.us/download)
13. Install [Slack](https://www.slack.com/downloads/windows)

# other things?

# Speedy 'nix tricks
- Digital color meter: https://alternativeto.net/software/digitalcolor-meter/?platform=linux
- GNOME Screenshot and Screencast ships with Ubuntu: https://help.ubuntu.com/stable/ubuntu-help/screen-shot-record.html
- use the `nautilus` command to open files in Gnome's desktop file manager, Nautilus, e.g. `nautilus` to open the working directory.

# Chrome magic
- React Developer Tools plugin.
- Redux Developer Tools plugin.
- One Tab plug-in to minimize open tabs into a list of URLs
- HTTPS everywhere (Ad Blocker? From EFF.
- `ctrl + l` focuses to the Location Bar.
- ctrl+option+ left right arrow to cycle through open tabs???

# Text Editor efficiency
