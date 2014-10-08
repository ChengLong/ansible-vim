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
I recommend using `ansible_ssh_user` and `ansible_sudo_pass` in your inventory. E.g. 

```
[test]
xxx.xxx.xxx.xxx ansible_ssh_user=exampleuser ansible_sudo_pass='password of exampleuser'
```

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
    - { role: ChengLong.vim }
```

License
-------

MIT

Author Information
------------------

[Cheng Long](https://twitter.com/ChengLong_)
