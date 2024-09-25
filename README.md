## setup ansible

```
/usr/bin/python3 -m pip install --user pipx
/usr/bin/python3 -m pipx ensurepath
pipx install --include-deps ansible
pipx upgrade --include-injected ansible
```

## run ansible

```
(ansible-galaxy install -r requirements.yml)
(ansible-playbook -v main.yml --ask-become-pass)
```

## setup GitHub

```
gh auth login
```
