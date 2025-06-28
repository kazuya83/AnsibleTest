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

## install手順　(MacOS)
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

## マネージドノードの要件
* python2.6以上、またはPython3.5以上
* SSH接続、ファイル転送方式としてSFTPまたはSCP

## プライブック
自動化したいマネージドノードへの処理をYAML形式で定義したファイル。Ansibleで自動化の仕組みを実装していく上で、、医術する時間が一番長くなるのがプレイブック。
プライブックはいくつかのセクションに分かれており、「hosts」には、操作対象の反映を指定する・

### プレイブック実行コマンド例
```
ansible-playbook -i inventory.ini playbool.yml
```