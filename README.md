# Virtualenvs the right way #

I like the philosophy of Pipenv, but I want to stay detached from the installation process and creation of the virtualenv. V solves that.


## Usage ##

Enter the virtualenv in a subshell:

```
$ cd ~/src/myproject
$ V enter
Virtualenv location: /home/user/src/myproject/.virtualenv
Python 3.7.6
Loading configuration file: .env
Type "exit" or press CTRL-D to exit
$ 
```


Exit the virtualenv (without closing the terminal):

```
$ exit
```


Show where the current directory's virtualenv lives:

```
$ cd ~/src/myproject
$ V where
/home/user/.local/share/virtualenvs/myproject_831ce98
```


Type `$ V` in your command line to see more examples.


## Installation

Put its directory in your PATH.

As a convenience, just type `$ ./install.sh` to symlink `V` to `~/.local/bin`.
