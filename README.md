Ansible Role for Vim 
=========

This role:

- install Vim
- copy [my .vimrc](https://raw.github.com/ChengLong/configs/master/.vimrc) to ~/.vimrc
- install Pathogen
- install Solarized
- install Nerdtree 
- install AutoComplPop

Requirements
------------

Please note that the task 'Install Dependencies' requires sudo. Please make that the user that your control machine ssh into has *sudo access*. 
I recommend using `ansible_ssh_user` and `ansible_ssh_user` in your inventory file, e.g.

```
[test_server]
xxx.xxx.xxx.xxx ansible_ssh_user=exampleuser 
```

You can use `--ask-sudo-pass` when running your playbook

`ansible-playbook playbook.yml -i inventory.ini --ask-sudo-pass`

Role Variables
--------------

NONE

Dependencies
------------

NONE

Example Playbook
----------------

```
- hosts: servers
  roles:
    - role: ChengLong.vim
```

License
-------

[WTFPL](http://www.wtfpl.net/). See WTFPL

Author Information
------------------

[Cheng Long](https://twitter.com/ChengLong_)
