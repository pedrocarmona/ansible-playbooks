# My Ansible


# Create ansible virtualenv

In command line:

```bash
brew install python

easy_install pip

pip install virtualenv

pip install virtualenvwrapper
```

Edit ~/.zshrc and add virtualenvwrapper to plugins:

```
plugins=(git rails ruby nmap tmux tmuxinator vagrant xcode zsh-completions virtualenvwrapper)
```

Restart command line, and after that:

```
mkdir -p ~/Developer/ansible

cd ~/Developer/ansible

mkvirtualenv ansible -a $(pwd)
```


Now everytime you run this command you automatically shift path to ~/Developer/ansible
```
workon ansible
```

And

```
which python
```

will point to /Users/youruser/.virtualenvs/ansible/bin/python

```
pip install ansible
```


