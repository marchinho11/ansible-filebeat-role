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

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: filebeat_role }
