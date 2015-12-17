# ansible playbook 
#adding linux user and setup ssh-keygen

[qiita](http://qiita.com/komitomo/private/e78855fa1ccee1737ac7) 

## put linux user name to playbook.yml

```playbook.yml
  vars:
    - username:  #put username
```


## add hosts IP address and login info to hosts file

```:hosts
[web]
#put IP here

[all:vars]
ansible_ssh_user=
ansible_ssh_private_key_file=
```

## run ansible-palybook command

```
ansible-playbook -i hosts playbook.yml
```
