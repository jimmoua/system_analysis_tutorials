
<h1>System Analysis and Design Dev Guide</h1>
Here are some basic tutorials/guides that may come in handy during your projects. These docs contains some of the tech that I've been using for development in other classes as well as other software that I personally use or find extremely helpful.

<h1>Table of Contents</h1>

- [Guides](#guides)
- [Personal Software of Choice](#personal-software-of-choice)
  - [Chocolatey (Windows)](#chocolatey-windows)
  - [Terminal](#terminal)
  - [Text Editor (GUI)](#text-editor-gui)
  - [Text Editor (CLI)](#text-editor-cli)
  - [Source Control Management](#source-control-management)

# Guides
- [A very basic tutorial on how to use Git and GitHub](git_github.md)
- [Amazon Web Services for Databases](AWS_rds.md)
- [Installing NodeJs](node_version_manager.md)
- [Installing MariaDB](mariadb_install.md)

# Personal Software of Choice
Below are some of the software that I use and personally recommend when doing development of any kind. **These personal recommendations are tech-stack agnostic, so whether you're working with a web application, an embedded system, or a kernel, you should be fine.** The shell commands that I use for installing below are only for the Chocolatey package manager on Windows. Since there are so many Linux distros, not all of them have the same package manager, so if you are using a Linux-based OS, you'll just have to figure out if your package manager source repos contain the software (chances are they will).

## Chocolatey (Windows)
Chocolatey is a package manager. Package managers are software will manage any other software that you install with it. This includes text editors, compilers, web browsers, software dependencies, and much more. You can't install all the software in the world with it, but you can install the most major software that are out there.

It is honestly such a good package manager for Windows and makes development setup on Windows so much more easier. Installing it is very easy, since you just need to paste in a single command into an terminal running on administrator rights. See (https://chocolatey.org/docs/installation) for installation.

## Terminal
I prefer [Alacritty](https://github.com/alacritty/alacritty) for my terminal emulator.

> Alacritty is the fastest terminal emulator in existence. Using the GPU for rendering enables optimizations that simply aren't possible without it. Alacritty currently supports macOS, Linux, BSD, and Windows.

It's also available in the Chocolatey package repositories, so you can install it using:

```
$ choco install alacritty
```

Depending on which Linux distro you are using, Alacritty isn't always available by default in all package managers. You may have to update your package sources or compile from source. See installation guide on their GitHub repo [here](https://github.com/alacritty/alacritty#installation).

## Text Editor (GUI)
My main editor of choice is [Visual Studio Code](https://code.visualstudio.com/). **It is NOT an IDE**, but you can configure it to where it basically is an IDE via plugins.

```
$ choco install vscode
```

## Text Editor (CLI)
If I need to do any quick edits on the command line, I will use [Neovim](https://neovim.io/). You can also install plugins for it which makes it highly customizable.

```
$ choco install neovim
```

## Source Control Management
I prefer Git, and I am going to make a bold claim that it's a de-facto for many. There is already a guide I have written on how to use it. [Here](git_github.md). You can install it using choco `$ choco install git`.