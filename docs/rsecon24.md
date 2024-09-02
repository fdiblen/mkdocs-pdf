# :snake: RSECon24 Workshop: Effortlessly creating Python packages with good practices

!!! info Session

    Time: 14:30-15:45 Tuesday, 3 September, 2024

    Location: 2.16 (Classroom)

    [Submission link](https://virtual.oxfordabstracts.com/#/event/49081/submission/99)

!!! note

    These notes are for the presenter and may change.

---
## :watch: 4 mins - Introduction - Presentation


---
## :watch: 1 min - Check the requirements

Instructions can be found at [https://github.com/fdiblen/RSECon24](https://github.com/fdiblen/RSECon24)

Check the shell

``` { .sh .copy .select linenums="0" title="" }
$ echo $SHELL
/usr/bin/bash
```

Check Python version

``` { .sh .copy .select linenums="0" title="" }
$ python --version
Python 3.12.5
```

Check git version

``` { .sh .copy .select linenums="0" title="" }
$ git --version
git version 2.46.0
```

GitHub account

``` sh linenums="0" title=""
$ ssh git@github.com
Hi fdiblen! You've successfully authenticated, but GitHub does not provide shell access.
Connection to github.com closed.
```

**Useful Links:**

- To create a new account: [https://github.com/signup](https://github.com/signup)
- To connect to GitHub with SSH: [https://docs.github.com/en/authentication/connecting-to-github-with-ssh](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)

---
## :watch: 14:35 (10 mins) - Create a Python package using a minimum profile

Install copier

``` { .sh .copy .select linenums="0" title="" }
python3 -m pip install --user pipx
python3 -m pipx ensurepath
pipx install copier
```

!!! info

    We will create a package called `baklava`


Create a new package by running:

``` { .sh .copy .select linenums="0" title="" }
copier copy https://github.com/nlesc/python-template.git baklava
```

Answer the questions as shown below:

```
Thanks for generating a project using our template.

You'll be asked a series of questions whose answers will be used to
generate a tailored project for you.

For each question there is a placeholder. Make sure you provide an
input to each of them.

🎤 Select a profile
   Minimum (bare minimum, no extra features)
🎤 Enter the name of the Python package.
   baklava
🎤 Enter the version of the Python package
   0.1.0
🎤 Enter your full name
   Faruk D
🎤 license
   Apache License, Version 2.0
🎤 Short description of package
   A sweet package
🎤 Add keywords to make your package findable on PyPI
   sweet,dessert
🎤 Enter the name of your GitHub username or organization
   fdiblen
🎤 What is your email address?
   f.diblen@esciencecenter.nl
🎤 Who is the copyright holder (the default is your full name)?
   Faruk D

Copying from template version None
    create  .
    create  NOTICE
    create  src
    create  src/baklava
    create  src/baklava/__init__.py
    create  src/baklava/my_module.py
    create  .copier-answers.yml
    create  MANIFEST.in
    create  README.md
    create  LICENSE
    create  .gitignore
    create  project_setup.md
    create  pyproject.toml

Your project "baklava" has been successfully created in baklava folder!

```

---
## :watch: 14:45 (5 mins) - Explain the generated files with minimum profile


```
├── LICENSE
├── MANIFEST.in
├── NOTICE
├── project_setup.md
├── pyproject.toml
├── README.md
└── src
    └── baklava
        ├── __init__.py
        └── my_module.py
```

---
## :watch: 14:50 (20 mins) - Update the new Python package

Add new features to the created package

``` { .sh .copy .select linenums="0" title="" }
copier copy https://github.com/nlesc/python-template.git baklava
```

```
```

---
## :watch: 15:10 (10 mins) - Create a new GitHub repository

Go to: https://github.com/new

- Repo name: baklava
- Description: `sweet Python package`
- Type: Public
- **NO README**
- **NO .gitignore**
- **NO license**


---
## :watch: 15:20 (15 mins) - Push the package to the new GitHub repository

- Look at the generated `next steps` issues
- Look at the workflows


---
##  :watch: 15:35 (10 mins) -  Feedback session

