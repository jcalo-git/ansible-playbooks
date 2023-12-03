# macOS Update Playbook

This Ansible playbook is designed to update a macOS machine. It performs the following tasks:

1. Checks if Homebrew is installed on the machine.
2. If Homebrew is not installed, it installs Homebrew.
3. Updates Homebrew.
4. Upgrades all installed Homebrew packages.
5. Checks for any available system updates.

## Usage

To run this playbook, you need to have Ansible installed on your machine. You can then run the playbook using the following command:

```ansible-playbook osx-weekly-patches.yml```

## If you would like to modify this to run from a central control node. Modify hosts and comment out connection. 

```
---
- name: Update OSX machines
  hosts: OSX # target group 
  gather_facts: false 

```