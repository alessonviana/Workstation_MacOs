# Workstation Tools

This repository contains scripts to automate and speedup the workflow and preparation for my machine.

> **_Disclaimer_** :
> Those scripts are macos, for other distributions you'll need to adapt it
___

## Prepare Workstation

> Read the `workstation.yaml` file before applying and be sure to understand everything that will be done.

1. Install Ansible
```bash
$ curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
```
```bash
$ pip install --user ansible
```

2. Clone this repository
```bash
$ git clone https://github.com/alessonviana/Workstation_MacOs.git
```

3. Apply the configuration
```bash
$ ansible-playbook workstation.yaml -i hosts.ini --ask-become-pass
```

>Type your password when asked to give root permissions for some actions.


### Tags that can be used in playbook:
    - update
    - chrome
    - docker 
    - git
    - spotifi
    - terraform 
    - kubectl
    - kubectx 
    - packages 
    - slack 
    - vscode
___

# License
GPLv3

# Author Information
Created by [@bergpb](https://twitter.com/lbergpb) </br>
Edit by [@alessonviana](https://alessonviana.tech)

Contributions are more than welcome!