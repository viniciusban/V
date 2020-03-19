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
