Ansible playbooks
=================

Usual and casual tasks for development debian server setting using ansible.

Roles
-----

This playbook install the following [1] :

#### System
  - [Basic packages and upgrade](roles/common) system
  - [Network Time Protocl](roles/ntp)
  - [Git distributed version control](roles/git) system
  - [Python](roles/python) programming language
  - [rmate](roles/rmate) tool
  - [Ferm](roles/ferm) tool
  - [ZSH](roles/zsh) shell

#### Monitoring
  - [Collectd](roles/collectd) tool
  - [Scout Realtime](roles/scout_realtime) tool

#### PHP
  - [PHP Fast Process Manager](roles/php-fpm) or [PHP Apache module](roles/php-apache) or [HipHop Virtual Machine](roles/php-hhvm)
  - [PHP useful extensions](roles/php-extensions)
  - [PHP Maxmind](roles/php-maxmind-geoip) extension
  - [PHP New Relic](roles/php-newrelic) extension
  - [PHP Phalcon](roles/php-phalcon) extension
  - [PHP 0MQ](roles/php-zmq) extension
  - [Composer](roles/composer) tool

#### Web server
  - [Apache](roles/apache) server or [Nginx](roles/nginx) server

#### Database
  - [MySQL](roles/mysql) server
  - [MariaDB](roles/mariadb) server
  - [Cassandra](roles/cassandra) server
  - [MongoDB](roles/mongodb)

#### Cache
  - [Memcached](roles/memcached) server
  - [Redis](roles/redis) server

#### Misc
  - [Bind](roles/bind) server
  - [Java](roles/java)
  - [Elasticsearch](roles/elasticsearch) server
  - [Postfix](roles/postfix) server
  - [Sharedance](roles/sharedance) server
  - [0MQ](roles/zeromq) server




[1] In fact, it MAY : You have to comment some playbook lines in order to bypass the unrequested roles.