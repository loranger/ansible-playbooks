Ansible playbooks
=================

Usual and casual tasks for development debian server setting using ansible.

Roles
-----

This playbook install the following [1] :

  - [Basic packages and upgrade](roles/common) system
  - [Network Time Protocl](roles/ntp)
  - [Git distributed version control](roles/git) system
  - [rmate](roles/rmate) tool
  - [PHP Fast Process Manager](roles/php-fpm) or [PHP Apache module](roles/php-apache) or [HipHop Virtual Machine](roles/php-hhvm)
  - [PHP useful extensions](roles/php-extensions)
  - [PHP Maxmind](roles/php-maxmind-geoip) extension
  - [PHP New Relic](roles/php-newrelic) extension
  - [PHP Phalcon](roles/php-phalcon) extension
  - [PHP 0MQ](roles/php-zmq) extension
  - [Composer](roles/composer) tool
  - [Nginx](roles/nginx) server
  - [MySQL](roles/mysql) server
  - [Cassandra](roles/cassandra) server
  - [Python](roles/python) programming language
  - [Sharedance](roles/sharedance) server
  - [Redis](roles/redis) server
  - [Elasticsearch](roles/elasticsearch) server
  - [Scout Realtime](roles/scout_realtime) tool
  - [0MQ](roles/zeromq) server




[1] In fact, it MAY : You have to comment come playbook lines in order to bypass the unrequested roles.