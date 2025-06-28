# AnsibleTest
<img src="https://img.shields.io/badge/-Ansible-000000.svg?logo=ansible&style=plastic">

## install手順 (Linux)
```
$ sudo dnf install python39 -y
$ python3.9 -m venv myvenv
$ source myvenv/bin/activate
$ pip install pip --upgrade
$ pip install ansible==4.2.0
```

# install手順　(MacOS)
```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
$ brew install python@3.9
$ python3 -m venv myvenv
$ source myvenv/bin/activate
$ pip3 install --upgrade pip
$ pip3 install ansible==4.2.0
```

## ansible version確認
```
ansible --version
```