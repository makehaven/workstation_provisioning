# workstation_provisioning

## Windows Workstation prep
On the Windows Workstations that will be provisioned by Ansible:
```
@powershell -NoProfile -ExecutionPolicy Bypass -Command "iex ((new-object net.webclient).DownloadString('https://github.com/ansible/ansible/raw/devel/examples/scripts/ConfigureRemotingForAnsible.ps1'))"
```

## Linux Control Machine (should work on MacOS, but I haven't tried it)

### Install Ansible see https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

For Ubuntu 18.04
```
$ sudo apt update
$ sudo apt install software-properties-common
$ sudo apt-add-repository --yes --update ppa:ansible/ansible
$ sudo apt install ansible
```
