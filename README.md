[![Galaxy](https://img.shields.io/badge/galaxy-dockpack.base__docker-blue.svg?style=flat)](https://galaxy.ansible.com/dockpack/base_docker)[![Build Status](https://api.travis-ci.org/dockpack/base_docker.svg)](https://travis-ci.org/dockpack/base_docker)

=========

## dockpack.base_docker is a role to install docker.

Requirements
------------

RHEL-like systems


Role Variables
--------------
To add additional user to the docker group declare and define

    docker_users:
      - jenkins
      - vagrant


Dependencies
------------
    []

Example Usage
----------------

    - name: Install docker on RedHat
      hosts: all
      become: 'True'

      roles:
      - {role: docker, tags: 'docker'}

License
-------

MIT

Author Information
------------------

Bas Meijer
@bbaassssiiee
