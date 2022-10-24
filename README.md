# ansible-deploy-vmware-vm

## Introduction

This project is a Ansible playbook to automate the deployment and configuration of VMs running on VMware vSphere. The `ansible-deploy-vmware-vm` project used Ansible `vmware_guest` module. This module can be used to create new virtual machines from templates or other virtual machines, manage power state of virtual machine such as power on, power off, suspend, shutdown, reboot, restart etc., modify various virtual machine components like network, disk, customization etc., rename a virtual machine and remove a virtual machine with associated components.

## Requirements

To use `ansible-deploy-vmware-vm` project you need to some packages in your Ansible machine. The requirements are as follows:

* python >= 2.6
* PyVmomi

By default Python installed on all Linux distributions, but maybe you need to install `PyVmomi` package. If you use the Fedora / RHEL / CentOS Linux, you can run below command:

```bash
sudo dnf install python3-pyvmomi
```

Or you can use a generic method to install it:

```bash
pip3 install pyvmomi
```

## Deploy

To deploy VM on VMware vSphere, after clone the project in your Ansible machine, enter information of your environment in variable file:

```bash
vi group_vars/all
```

Now for running Ansible Playbook you should run the beneath command:

```bash
ansible-playbook  main-playbook.yml
```

## Contact

[Project website: "https://github.com/hos7ein/ansible-deploy-vmware-vm"]

[Personal website: "https://fedorafans.com"]

**Author**: Hossein Aghaie <hossein.a97@gmail.com>

**Twitter**: Hossein Aghaie [@hos7ein](https://twitter.com/hos7ein)

## License

`ansible-deploy-vmware-vm` source code is available under the GPL-3.0 [License](/LICENSE).
