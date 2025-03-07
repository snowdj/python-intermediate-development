---
title: Setup
---

You will need the following software installed and working correctly on your system to be able to follow the workshop.

## Command Line Program
You can use a command line program such as [Bash](https://www.gnu.org/software/bash/). 
If you already have a command line program other than Bash - you can use that 
instead as none of the content of this workshop is specific to Bash.
  - On Windows, Bash will be installed as part of Git Bash (included in [Git For Windows package](https://gitforwindows.org/) - see Git installation section below)  
  - On macOS and Linux, you will already have a command line program available (note that starting with macOS Catalina, 
Macs will use [Zsh (Z shell)](https://www.zsh.org/) as the default shell instead of Bash)

To test the installation, start your command line/Git Bash program and type:
~~~
$ date
~~~
{: .language-bash}

If your command line program is working - it should return the current date and time similar to:
~~~
Wed 21 Apr 2021 11:38:19 BST
~~~
{: .output}
  
## Git Version Control Tool
Git is a program that can accessed via the command line.

  - On Windows, you will need Git Bash, which comes included as part of the [Git For Windows package](https://gitforwindows.org/) and will 
  install the Bash shell as well as Git 
  - On macOS, Git is included as part of Apple's [Xcode tools](https://en.wikipedia.org/wiki/Xcode) 
and should be available from the command line as long as you have XCode. If you do not have XCode installed, you can download it from 
[Apple's App Store](https://apps.apple.com/us/app/xcode/id497799835?mt=12) or you can 
[install Git using alternative methods](https://git-scm.com/download/mac).
  - On Linux, Git can be installed using your favourite package manager

To test your Git installation, start your command line/Git Bash program and type:
~~~
$ git help
~~~
{: .language-bash}

If your Git installation is working you should see something like:
~~~
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
$ git help
~~~
{: .output}

### GitHub Account                     
For the purposes of the course, you will also need a [GitHub](https://github.com/) account. 
GitHub is a free, online host for Git repositories that you will use during the course to store your code in. 
You can create an account at [GitHub](https://github.com/) for free if you don't already have one.

## Python Distribution
The material has been developed using the [standard Python distribution version 3.8](https://www.python.org/downloads/) 
and is using `venv` for virtual environments and `pip` for package management. 
The material has not been extensively tested with other Python distributions and package managers, 
but most sections are expected to work with some modifications. 
For example, package installation and virtual environments would need to be managed differently, but Python script 
invocations should remain the same regardless of the Python distribution used.

To download a Python distribution for your operating system,
please head to [Python.org](https://www.python.org/downloads/).
>## Recommended Python Version
> We recommend using Python version 3.3+ since `venv` will be included in the Python standard library and requires 
> no additional installation. Things won't work well if you use Python 2.
{: .callout}

You can 
test your Python installation from the command line with:
~~~
$ python3 --version
~~~
{: .language-bash}
If all is well with your installation, you should see something like:
~~~       
Python 3.8.2
~~~
{: .output}

To make sure you are using the standard Python distribution and not some other distribution you may have on your system, 
 type the following in your shell:
 ~~~
 $ python3
 ~~~
 {: .language-bash}
This should enter you into a Python console and you should see something like:
 ~~~
Python 3.8.2 (default, Jun  8 2021, 11:59:35) 
[Clang 12.0.5 (clang-1205.0.22.11)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> 
 ~~~
 {: .language-bash}
 Press `CONTROL-D` to exit the Python console.

### `venv` and `pip`
If you are using a Python 3 distribution from [Python.org](https://www.python.org/), 
`venv` and `pip` will be automatically installed for you. If not, please make sure you have these
two tools (that correspond to your Python distribution) installed on your machine.

## PyCharm IDE
We use JetBrains's [PyCharm Python Integrated Development Environment](https://www.jetbrains.com/pycharm) for the course. 
PyCharm can be downloaded from [the JetBrains website](https://www.jetbrains.com/pycharm/download).
The Community edition is fine, though if you are developing software for the purpose of academic research you may 
be eligible for a free license for the Professional edition which contains extra features
  
{% include links.md %}
