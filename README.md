# [vim](#vim)

Install vim on your system.

|GitHub|GitLab|Quality|Downloads|Version|Issues|Pull Requests|
|------|------|-------|---------|-------|------|-------------|
|[![github](https://github.com/buluma/ansible-role-vim/workflows/Ansible%20Molecule/badge.svg)](https://github.com/buluma/ansible-role-vim/actions)|[![gitlab](https://gitlab.com/buluma/ansible-role-vim/badges/master/pipeline.svg)](https://gitlab.com/buluma/ansible-role-vim)|[![quality](https://img.shields.io/ansible/quality/57964)](https://galaxy.ansible.com/buluma/vim)|[![downloads](https://img.shields.io/ansible/role/d/57964)](https://galaxy.ansible.com/buluma/vim)|[![Version](https://img.shields.io/github/release/buluma/ansible-role-vim.svg)](https://github.com/buluma/ansible-role-vim/releases/)|[![Issues](https://img.shields.io/github/issues/buluma/ansible-role-vim.svg)](https://github.com/buluma/ansible-role-vim/issues/)|[![PullRequests](https://img.shields.io/github/issues-pr-closed-raw/buluma/ansible-role-vim.svg)](https://github.com/buluma/ansible-role-vim/pulls/)|

## [Example Playbook](#example-playbook)

This example is taken from `molecule/default/converge.yml` and is tested on each push, pull request and release.
```yaml
---
- hosts: all
  vars:
    ansible_python_interpreter: /usr/bin/python3
    wp_version: 6.0.1
    wp_mysql_db: 'database_name_here'
    wp_mysql_user: 'username_here'
    wp_mysql_password: 'password_here'
    wp_webserver: nginx
    wp_sitename: localhost
    wp_admin_email: 'admin@example.com'
    wp_install_dir: "/var/www/{{ wp_sitename }}"
  roles:
    - buluma.wordpress
```


## [Role Variables](#role-variables)

The default values for the variables are set in `defaults/main.yml`:
```yaml
---
# defaults file for vim
plugins:
  - name: vim-airline
    url: https://github.com/vim-airline/vim-airline
  - name: nerdtree
    url: https://github.com/preservim/nerdtree
  - name: fzf-vim
    url: https://github.com/junegunn/fzf.vim
  - name: vim-gitgutter
    url: https://github.com/airblade/vim-gitgutter
  - name: vim-fugitive
    url: https://github.com/tpope/vim-fugitive
  - name: vim-floaterm
    url: https://github.com/voldikss/vim-floaterm
```

## [Requirements](#requirements)

- pip packages listed in [requirements.txt](https://github.com/buluma/ansible-role-vim/blob/main/requirements.txt).


## [Context](#context)

This role is a part of many compatible roles. Have a look at [the documentation of these roles](https://buluma.github.io/) for further information.

Here is an overview of related roles:

![dependencies](https://raw.githubusercontent.com/buluma/ansible-role-vim/png/requirements.png "Dependencies")

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://hub.docker.com/u/buluma):

|container|tags|
|---------|----|
|fedora|34, 35, 36|
|opensuse|all|
|ubuntu|all|

The minimum version of Ansible required is 2.10, tests have been done to:

- The previous version.
- The current version.
- The development version.



If you find issues, please register them in [GitHub](https://github.com/buluma/ansible-role-vim/issues)

## [Changelog](#changelog)

[Role History](https://github.com/buluma/ansible-role-vim/blob/master/CHANGELOG.md)

## [License](#license)

Apache-2.0

## [Author Information](#author-information)

[Michael Buluma](https://buluma.github.io/)
