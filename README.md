# Getting-Started

### NOTES
- https://lambdaschoolstudents.slack.com/archives/G8W8LT9SM/p1518711817000364
- $PATH walkthrough?

### Minimum hardware requirements?
- 2GHz processor (?)
- 8GB RAM

### Adequate storage for Lambda School projects and requisite tools (~5GB)
| Tool | Storage | Cost |
|---|---|---|
| Lambda School projects | ~1GB | Free |
| Chrome | ~400MB | Free |
| GitBash (Windows) | ??? | Free |
| NodeJS | ~60MB | Free |
| NodeJS packages | including `create-react-app`, `lessc`, `nodemon`, `yarn` | Free |
| Text Editor | (see table below) | Free |
| Zoom | ~30MB | Free |
| Slack | ~220MB | Free |
| PostMan | ~260MB | Free |
| MongoDB & mongod | ??? | Free |
| MongoDB GUI | Robo 3T ~60MB, Workbench ?) | Free |

| Text Editor | Application Size | Cost |
|---|---|--:|
| Vim | ~  2MB | Free |
| Sublime | ~ 30MB | Free nagware<sup>*</sup> or $80US per single user |
| Emacs | ~ 50MB | Free |
| VSC | ~200MB | Free |
| Atom | ~500MB | Free |

<sup>*</sup> https://www.sublimetext.com/buy Sublime is a great text editor. The free version is fully-functional. It will occasionally remind to to buy a license (i.e. "nagware"). Licenses are per user, not per machine. If you like it, why not let Jon Skinner and Will Bond know by buying a license?

# Objectives
Once you have downloaded the NodeJS installer and have installed NodeJS on your computer you will have _both_ the `node` and `npm` commands available. Launch your console. NOTE: it is a convention to use the dollar sign `$` to indicate the console prompt. You want to use the commands which follow this prompt - do not enter `$` into the console. Nothing bad will happen, but the console (i.e. terminal, shell) won't know what to make of it. That said, you can confirm that the `node` and `npm` commands are installed like so:

```console
$  node -v
    v8.11.1
$  npm -v
    5.6.0
```

Now use the NodeJS Package Manager (`npm`) to install some additional NodeJS packages. With the following command, the `i` is short for **"i"**nstall (you could spell out `install` but you can save six whole keystrokes!) The `-g` flag let's the `npm` command know to install these packages **"g"**lobally on your system.

```console
$ npm i -g create-react-app less nodemon yarn
```

If you get warnings and errors about permissions, you may need to invoke this command by prepending it with `sudo` - the **"s"**uper**"u"**ser **"do"** command. This will allow the command to be run with more security privileges. You will be prompted for your password.

By the time you complete the setup for your particular operating system you should be able to confirm that the following tools are installed on your machine and available through your environment's $PATH:

```console
$  node -v
    v8.11.1
$  npm -v
    5.6.0
$  create-react-app --version
    1.5.2
$  lessc -v
    lessc 3.0.1 (Less Compiler) [JavaScript]
$  nodemon -v
    1.17.3
$  yarn -v
    1.5.1
$  mongod --version
    db version v3.6.3
    git version: 9586e557d54ef70f9ca4b43c26892cd55257e1a5
    OpenSSL version: OpenSSL 1.0.2o  27 Mar 2018
    allocator: system
    modules: none
    build environment:
        distarch: x86_64
        target_arch: x86_64
```

NOTE: these version numbers may be different than yours.

# Sign Up!
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
