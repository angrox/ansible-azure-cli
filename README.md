# Azure-CLI

[![Build Status](https://travis-ci.org/angrox/ansible-azure-cli.svg?branch=master)](https://travis-ci.org/angrox/ansible-azure-cli)


This role installs the Azure CLI on a CentOS/RHEL maschine using python pip. The CLI needs python > 3 so we need to install the SCL python version.

## Variables
* installation_method: Install as 'rpm' or via 'pip'. Defaults to 'rpm'
* scl_python_version: Version of SCL python, defaults to 35 (only used with pip installation method)
* upgrade_azure_cli: Call pip with --upgrade. Default to false (only used with pip installation method)

## Usage
Example playbook:
```
- hosts: all
  roles:
    - role: angrox.azure-cli
```

