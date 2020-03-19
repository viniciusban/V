# Virtualenvs the right way #

I like the philosophy of Pipenv, but I want to stay detached from the installation process and creation of the virtualenv. V solves that.


## Usage ##

To enter the virtualenv:

```
$ cd ~/src/myproject
$ V enter $PWD/.virtualenv
Virtualenv location: /home/user/src/myproject/.virtualenv
Python 3.7.6
Loading configuration file: .env
Type "exit" or press CTRL-D to exit
$ 
```


To exit the virtualenv:

```
$ exit
```

It will not close your terminal because V opens a subshell for the virtualenv.


To show where the current directory's virtualenv lives:

```
$ cd ~/src/myproject
$ V where
/home/user/.local/share/virtualenvs/myproject_831ce98
```


To generate virtualenv path for the current directory:

```
$ cd ~/src/myproject
$ V gen
/home/user/.local/share/virtualenvs/myproject_831ce98
```

It is useful when creating a new virtualenv:

```
$ python -m venv $(V gen)
$ V enter
Virtualenv location: /home/user/.local/share/virtualenvs/myproject_831ce98
Python 3.7.6
Type "exit" or press CTRL-D to exit
$ 
```
