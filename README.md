Ansible playbooks
=================

Usual and casual tasks for development debian server settings using [ansible galaxy](https://galaxy.ansible.com/intro)

Roles
-----

This playbook install the following [1] :

#### System
  - [Basic packages and upgrade](roles/common) system
  - [Network Time Protocl](roles/ntp)
  - [Git distributed version control](roles/git) system
  - [Python](roles/python) programming language
  - [Go](roles/go) programming language
  - [rmate](roles/rmate) tool
  - [Ferm](roles/ferm) tool
  - [ZSH](roles/zsh) shell
  - [Prezto](roles/prezto) zsh enhancement
  - [Supervisor](roles/supervisor) daemon

#### Monitoring
  - [Collectd](roles/collectd) tool
  - [Scout Realtime](roles/scout_realtime) tool
  - [Packetbeat](roles/packetbeat) tool

#### PHP
  - [PHP Fast Process Manager](roles/php-fpm) or [PHP Apache module](roles/php-apache) or [HipHop Virtual Machine](roles/php-hhvm)
  - [PHP useful extensions](roles/php-extensions)
  - [PHP Maxmind](roles/php-maxmind-geoip) extension
  - [PHP New Relic](roles/php-newrelic) extension
  - [PHP Phalcon](roles/php-phalcon) extension
  - [PHP 0MQ](roles/php-zmq) extension
  - [PHP XDebug](roles/php-xdebug) extension
  - [Composer](roles/composer) tool

#### Web server
  - [Apache](roles/apache) server or [Nginx](roles/nginx) server

#### Database
  - [MySQL](roles/mysql) server
  - [MariaDB](roles/mariadb) server
  - [Cassandra](roles/cassandra) server
  - [MongoDB](roles/mongodb)
  - [InfluxDB](roles/influxdb) server
  
#### Queue messaging
  - [0MQ](roles/zeromq) server
  - [Beanstalkd](roles/beanstalkd) server

#### Cache
  - [Memcached](roles/memcached) server
  - [Redis](roles/redis) server
  
#### Image
  - [ImageMagick](roles/imagemagick) tool
  - [GraphicsMagick](roles/graphicsmagick) tool
  - [FaceDetect](roles/facedetect) tool

#### Search
  - [Elasticsearch](roles/elasticsearch) server
  - [Sphinx](roles/sphinxsearch) server

#### Misc
  - [HAProxy](roles/haproxy) load balancer
  - [Bind](roles/bind) server
  - [Java](roles/java)
  - [Kibana](roles/kibana) tool
  - [Postfix](roles/postfix) server
  - [PredictionIO](roles/predictionio) server
  - [Sharedance](roles/sharedance) server



[1] In fact, it MAY : You have to comment some playbook lines in order to bypass the unrequested roles. You could also add your own role or any [ansible galaxy role](https://galaxy.ansible.com/intro)