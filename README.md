K8S Keystone
=========
[![Galaxy](https://img.shields.io/badge/galaxy-tripleo.k8s--keystone-blue.svg?style=flat)](https://galaxy.ansible.com/tripleo/k8s-keystone)
[![Build Status](https://travis-ci.org/tripleo/ansible-role-k8s-keystone.svg?branch=master)](https://travis-ci.org/tripleo/ansible-role-k8s-keystone)

Install Keystone in a Kubernetes cluster.

Requirements
------------

Access to Kubernetes cluster

Role Variables
--------------

| Name              | Default Value       | Description          |
|-------------------|---------------------|----------------------|
| `action` | `provision` | List of tasks to run. |
| `coe_host` | |  |
| `coe_config_context` | |  |
| `coe_config_file` | |  |


Dependencies
------------

- `ansible.kubernetes-modules`

Example Playbook
----------------

    - hosts: all
      roles:
         - tripleo.k8s-keystone
