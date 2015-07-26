nginx
=====

free, open-source, high-performance HTTP server and reverse proxy, as well as an IMAP/POP3 proxy server

Supported Tasks
-----------------

The following tasks are executed :

  - Install [nginx](http://nginx.org/)
  - Setup minimal settings using nginx.conf and defaut enabled website
  - Enable PHP-FPM proxy and copy a simple phpinfo script

How to add your nginx sites
---------------------------

Create folder ```nginx-hosts``` beside ```ansible-playbooks``` and subfolders like in this example:


```
- your_environment/       # Some root, where you placed this project
                          # It can be independently controlled by git

- - ansible-playbooks/    # Folder with current project
                          # You can use 'git clone' for your fork
                          # and change it like you want
                          # Be careful with private information

- - nginx-hosts/          # ! You should create this directory and subfolders

- - - vars/               # Copy ansible-playbooks/role/nginx/vars/nginx_defaults.yml
                          # to nginx-hosts/vars/nginx_secrets.yml

- - - - nginx_secrets.yml # Configure your sites in this folder

- - - templates/          # If you need, place here a special
                          # *.conf.j2 files with non-default
                          # configuration for one or many sites
                          #
                          # Copy ansible-playbooks/role/nginx/templates/project_example.conf.j2
                          # to nginx-hosts/templates/yourhost.conf.j2

- - - - project.conf.j2   # just like this
- - - - another.conf.j2   # and/or this

- - Vagrantfile           # Maybe you use it
```

After this steps you will can commit your project files independently of ansible roles in private repository