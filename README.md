# 【MacOS】Django environment
I am assuming that already python is installed in your development environmet.

## Set up virtual environment(venv)
### Created a new application directory.
For this tutorial we will be using a new directory [sample_app] from your home directory.

```command-line
$ mkdir ~/sample_app   #=> make a sample_app directory in home direcory.
$ cd ~/sample_app   #=> change a home directory to sample_app.
```
### Make a virtualenv [myvenv]
We will make a virtualenv called myvenv.
```command-line
$ python3 -m venv myvenv
```
`myvenv` is the name of your virtualenv.

### Activate your virtual environment
Start your virtual environment by running.

```command-line
$ source myvenv/bin/activate
```

## Install Django
Now that you have your virtualenv started, you can install Django.
### Create a requirements file
Create a requirements.txt file inside of the sample_app/ directory.
```command-line
$ touch requirements.txt
```
And you should add the following text like this.
``` requirements.tx
Django~=2.2.4
```

### Installing Django
Run `pip install -r requirements.txt` to install Django.
``` command-line
$ pip install -r requirements.txt
Collecting Django~=2.2.4 (from -r requirements.txt (line 1))
  Using cached https://files.pythonhosted.org/packages/94/9f/a56f7893b1280e5019482260e246ab944d54a9a633a01ed04683d9ce5078/Django-2.2.5-py3-none-any.whl
Collecting sqlparse (from Django~=2.2.4->-r requirements.txt (line 1))
  Using cached https://files.pythonhosted.org/packages/ef/53/900f7d2a54557c6a37886585a91336520e5539e3ae2423ff1102daf4f3a7/sqlparse-0.3.0-py2.py3-none-any.whl
Collecting pytz (from Django~=2.2.4->-r requirements.txt (line 1))
  Using cached https://files.pythonhosted.org/packages/87/76/46d697698a143e05f77bec5a526bf4e56a0be61d63425b68f4ba553b51f2/pytz-2019.2-py2.py3-none-any.whl
Installing collected packages: sqlparse, pytz, Django
Successfully installed Django-2.2.5 pytz-2019.2 sqlparse-0.3.0
```

## Generate your Django project
### Create project
You should run the `django-admin startproject [project name] .`. Don't forget to add the period (or dot) . at the end!
For this tutorial we will be using a [sample_project] in project name. So you should change it
``` commando-line
$ django-admin startproject sample_project .
```


Installing packages with requirements
