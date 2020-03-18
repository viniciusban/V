# Virtualenvs the right way #

I like the philosophy of Pipenv, but I want to stay detached from the installation process and creation of the virtualenv. V solves that.


## Usage ##

You can create the virtualenv with your preferred tool. V only tells you where it is located:

```
$ mkdir ~/src/myproject
$ cd ~/src/myproject
$ python -m venv $(V path .)
```

V relies on the `V_PREFIX_DIR` environment variable to show you the path for your virtual environment. By default it is equal to `XDG_DATA_HOME/virtualenvs`.


To open a shell with the virtualenv activated:

```
$ cd ~/src/myproject
$ v shell
Entering the virtualenv in a subshell...
Virtualenv located at ~/.local/bin/share/virtualenvs/myproject_16804b4
Loading configuration file: .env
Virtualenv activated with Python 3.7.6
Type "exit" to leave this shell
$ 
```
