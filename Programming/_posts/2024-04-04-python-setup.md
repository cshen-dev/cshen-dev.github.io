---
layout: post
title: "Python Local Setup Cheatsheet"
tags: [beginner]
---

Python is a common runtime for many automation tasks, and local setup remains relevant even though you can containerize your scripts or applications — convenience is still king.

## Python version manager

- [pyenv/pyenv: Simple Python version management](https://github.com/pyenv/pyenv)
- [pyenv/pyenv-virtualenv: a pyenv plugin to manage virtualenv (a.k.a. python-virtualenv)](https://github.com/pyenv/pyenv-virtualenv)


## Commands

1. `brew install pyenv` (Installing via Homebrew is still the easiest option.)

2. You may need the following commands to enable pyenv to auto-load in your default shell environment.
```
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init - zsh)"' >> ~/.zshrc
```

3. `pyenv install -l` (List all available Python versions)

4. `pyenv install` (Install the Python version according to local `.python-version` file)

5. `pyenv local xxx` (Lock a Python version locally)

6. `brew install pyenv-virtualenv` (Install virtualenv to provide additional package isolation for each project.)

7. You may need the following commands to enable pyenv-virtualenv to auto-load in your default shell environment.
```
echo 'eval "$(pyenv virtualenv-init -)"' >> ~/.zshrc
``` 