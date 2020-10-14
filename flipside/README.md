# FlipSide

This repository contains the FlipSide [Django](https://docs.djangoproject.com/en/3.0/) WebApp.

### Tech References

Refer to these documentations if you want to read up on the technologies involved:
* [Django](https://docs.djangoproject.com/en/3.0/) - Python Web Framework v3.0 and later
* [VirtualEnv](https://pypi.org/project/virtualenv/) - VirtualEnv to encapsulate WebApp dependencies.
* [Python](https://www.python.org/downloads/) - Python v3.8 and later
* [Terminal Basic Commands](https://www.hostinger.com/tutorials/linux-commands) - Basic commands to navigate, install, etc... using Terminal.

### Installation

You need to install [Python v3.8+](https://www.python.org/downloads/)
Go to the Python.org website, and download any version from 3.8 to later.

##### Clone Repo

In order to get this repository on your machine, you need to create a GitHub Account, and install git on your machine.
Once the above is achieved, create a folder on your machine that will contain this project.
Open Terminal, run 
```sh 
$ cd /path/to/your/project/folder
```

Then run 
```sh 
$ git clone https://github.com/Mark223D/FlipSide.git
```

This will create a folder called `Flipside/`, containing 4 elements:
* `flipside/` is the main folder of the project.
* `README.md` is this file that you are readin right now.
* `manage.py` is the Python file that will run the Django App.
* `db.sqlite3` is a temporary light-weight `SQLite` database.

Run the following to enter into the directory:
```sh
$ cd FlipSide
```

##### Install virtualenv

After installing Python3, you will need to install ```virtualenv```.
Run the following to upgrade pip:
```sh
$ python3 -m pip install --upgrade pip
```

```Pip3``` is the Python Package Manager, which will handle all the dependencies, libraries, packages, etc... that  are needed.
Run the following to install virtualenv:
```sh
$ pip3 install virtualenv
```


Once the install is complete, you need to create a virtual environment in your project.
**Make sure you are NOT INSIDE the ```flipside/``` directory. You should be at the same level.**
Run the following to create a virtual environment.
```sh
$ virtualenv venv
```
This will create a folder called ```venv``` at the same level as the the ```flipside/``` directory.

Run the following to activate your virtual enviornment:
```sh
$ source venv/bin/activate
``` 
At this point, you should see `(venv)` prefixing your terminal command line (i.e. ` (venv) $`)

##### Install Required Packages

FlipSide contains a ```requirements.txt``` file that entails a brief description of all the dependencies needed for the project to run.
Later on, when libraries are added to the project they **should** be added to this file as well.

Thankfully, we can use this to not install every dependency manually (especially if they're many).

**Make sure you are at the same level as the ```requirements.txt``` file.**
**Make sure you are at that you (venv) is running**
Run the following to install all necessary dependencies.
```sh
(venv)$ pip install -r requirements.txt 
```

### Running Django Project

Once everything has been setup successfully, it's time to run the project.
To do that run the following:
**Make sure you are at the same level as the `manage.py` file**
```sh
(venv) $ python3 manage.py runserver
```
If all was successful, you should see in the output a link containing `localhost` or some IP address (i.e. `127.0.0.1`), go to this link in your browser to access website.

### Project Structure

The inital setup of the project is as follows:
```
FlipSide/
│───flipside/
    │───__init__.py
    │───__pycache__/(Server Cache)
    │───asgi.py(Settings extension)
    │───settings.py(Server settings)
    │───urls.py(Main URLS file)
    │───wsgi.py
│───README.md(This file)
│───manage.py(Server Runner)
└───db.sqlite3
```
Every component added to the project is an *`app`* in Django.
An app is, ideally, an independent module, with its own urls, business logic functions, data object.

Refer to [this link](https://www.youtube.com/watch?v=2-U4writF0I) to know more about Django File Structure and Django Apps


### References & Knowledge

* [Django](https://docs.djangoproject.com/en/3.0/) - Django Documentation
* [Project Structure](https://www.youtube.com/watch?v=2-U4writF0I) - How the file structure works
* [Terminal Basic Commands](https://www.hostinger.com/tutorials/linux-commands) - Basic commands to navigate, install, etc... using Terminal.







