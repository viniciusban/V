# Ve manages virtualenv. The right way #

I like the philosophy of Pipenv, but I want to stay detached from the installation process and creation of the virtualenv. Ve solves that.


## Usage ##

Enter the virtualenv in a subshell:

```
$ cd ~/src/myproject
$ ve shell
Virtualenv location: /home/user/.local/share/virtualenvs/myproject_831ce98
Python 3.7.6
Loading configuration file: .env
Loading configuration file: .env_override
Type "exit" or press CTRL-D to exit
$ 
```


Exit the virtualenv (without closing the terminal):

```
$ exit
```

Create a virtualenv:

```
$ cd ~/src/myproject
$ python -m venv $(ve gen)
/home/user/.local/share/virtualenvs/myproject_831ce98
```


Show where the current directory's virtualenv lives:

```
$ cd ~/src/myproject
$ ve where
/home/user/.local/share/virtualenvs/myproject_831ce98
```


Type `$ ve` in your command line to see the help.


## Installation

Put its directory in your PATH.

As a convenience, just type `$ ./install.sh` to symlink `ve` to `~/.local/bin`.
