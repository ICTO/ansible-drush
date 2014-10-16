Drush
=========

Ansible role to perform a very specific drush installation : the drush repo is cloned locally, dependencies are installed via the local
host and the complete dir is the rsync'ed to the remote host.

The purpose of this playbook is to enable installation of drush to remote hosts that have limited access to the internet,
or can't install the dependencies or drush via any other way.

Requirements
------------

No pre-requisites.

Role Variables
--------------

vars/main.yml :
* drush_repo
* drush_version

From group or host vars:
* drush_local_dir
* drush_remote_dir
