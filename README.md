Filebeat role
=========

Роль для установки filebeat на хостах с ОС: Debian, Ubuntu, CentOS, RHEL.

Requirements
------------

Поддерживаются только ОС семейств debian и EL.

Role Variables
--------------

| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| filebeat_version | "7.14.0" | Параметр, который определяет какой версии filebeat будет установлен |
| elastic_address | "0.0.0.0:9200" | Параметр, который определяет адрес elastic |
| kibana_address | "0.0.0.0:5601" | Параметр, который определяет адрес kibana |

Example Playbook
----------------
- hosts: all
  roles:
     - { role: filebeat_role }
