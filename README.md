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

Installing packages with requirements
