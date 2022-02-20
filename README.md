Filebeat role
=========

Роль для установки kibana на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и EL.

Role Variables
--------------

* filebeat_version (default: "7.14.0") - Параметр, который определяет какой версии filebeat будет установлен.
* Имя хоста Elasticsearch в шаблоне конфига filebeat [templates/filebeat.yml.j2](templates/filebeat.yml.j2), считывается из hostvars (default: 'el-instance').
* Имя хоста Kibana в шаблоне конфига filebeat [templates/filebeat.yml.j2](templates/filebeat.yml.j2), считывается из hostvars (default: 'ki-instance').

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: filebeat-role }

License
-------

MIT

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
