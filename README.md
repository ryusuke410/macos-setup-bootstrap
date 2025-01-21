# macos setup bootstrap

## setup brew path

edit `.zshrc`

```sh
# brew
export PATH="$PATH:/opt/homebrew/bin"
```

## setup ansible

```sh
xcode-select --install
/usr/bin/python3 -m pip install --user pipx
/usr/bin/python3 -m pipx ensurepath
pipx install --include-deps ansible
pipx upgrade --include-injected ansible
```

## git clone

clone this repository.

## run ansible

```sh
(ansible-galaxy install -r requirements.yml)
(ansible-playbook -v main.yml --ask-become-pass)
```

## setup GitHub

```sh
gh auth login
```
