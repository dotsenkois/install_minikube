install_minikube
=========

Роль устанавливает на хост UBUNTU >=20.04 LTS бинарники kubrctl, minikube а так же зависимости: docker.io, conntrack

Requirements
------------

none

Role Variables
--------------
defaults:
- kubernetes_version: "v1.24.1"   - Версия kubectl (внезапно). Необходима для скачивания бинарника
- minikube_install_type: remote   - тип установки
- pkg_tmp_src: "/tmp"             - временная папка для хранения бинарников


Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

---
- hosts: minikube
  roles:
    - install_minikube
    - k8s_run_hello_world

License
-------

BSD

Author Information
------------------

dotsenkois
Илья Доценко.
Специально для онлайн-школы netology.ru
