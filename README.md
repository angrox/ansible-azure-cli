# Azure-CLI

This role installs the Azure CLI on a CentOS/RHEL maschine using python pip. The CLI needs python > 3 so we need to install the SCL python version.


## Variables
* scl_python_version: Version of SCL python, defaults to 35
* upgrade_azure_cli: Call pip with --upgrade. Default to false

## Usage
Example playbook:
```
- hosts: all
  roles:
    - role: angrox.azure-cli
```

