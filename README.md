## Set up venv

```ruby
$ virtualenv -p `which python2.7` venv
$ source venv/bin/activate
$ pip install -r requirements.txt
```

## Install galaxy roles

```ruby
ansible-galaxy install -p ./roles/galaxy -r galaxy-requirements.yml

```

## Ansible Vault

```ruby
ansible-vault edit vars/secret.yml.vault
```

password is `1234ttt`

## Execute

```ruby
ansible-playbook -i vagrant.py --ask-vault-pass playbook.yml
```
and put valut password `1234ttt`
