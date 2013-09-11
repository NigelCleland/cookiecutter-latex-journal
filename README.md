cookiecutter-latex-journal
==========================

Templates for creating Journal Articles with LaTeX and Cookiecutter
See https://github.com/audreyr/cookiecutter

Key Points
----------

- Free Software: MIT License
- Multiple Article styles
    + IEEE Transactions
    + Elsevier
    + Plain (Vanilla LaTeX)
- Single Makefile for compiling


Usage
-----

- Clone the package
- Modify the cookiecutter.json file
- Generate the package

```
cookiecutter path/to/cookiecutter-latex-journal
```

- Create a repo (e.g. github or bitbucket)
- Add the remote and push the source

```
git init
git remote add origin https://github.com/user/repo.git
git add .
git commit -m "My first commit!"
git push -U origin master
```

- Work normally using git to manage different versions and features


Upcoming Features
-----------------

- More supported article types
- Smarter handling of author, date, titles etc between articles
- Multiple Authors from the cookie cutter
- IEEE bibliography creation
- Automated cleaning of LaTeX temporary files after build


