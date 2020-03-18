# Virtualenvs the right way #

I like the philosophy of Pipenv, but I want to stay detached from the installation process and creation of the virtualenv. V solves that.


## Usage ##

To enter the virtualenv:

```
$ cd ~/src/myproject
$ . v enter <path>
Saving current environment...
Virtualenv located at ~/.local/bin/share/virtualenvs/myproject_16804b4
Loading configuration file: .env
Virtualenv activated with Python 3.7.6
Type ". v exit" to leave it
$ 
```


To exit the virtualenv:

```
$ . v exit
Restoring previous environment...
Virtualenv exited
$ 
```

