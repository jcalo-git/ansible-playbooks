# Weekly Patches Playbook for Linux

These Ansible playbooks are designed to automate the process of updating and upgrading packages on Linux hosts. It performs the following tasks:

weekly-patches-selector.yml
1. Asks the user which host group they would like to apply patches on.
2. Updates the package lists for upgrades and new package installations.
3. Upgrades all the installed packages on the host.
4. Checks if the system requires a reboot after the upgrade.
5. If a reboot is required, it reboots the system.


weekly-patches.yml - complete automation across all machines in your hosts file
1. Updates the package lists for upgrades and new package installations.
2. Upgrades all the installed packages on the host.
3. Checks if the system requires a reboot after the upgrade.
4. If a reboot is required, it reboots the system.

## Usage

To run this playbook, you need to have Ansible installed on your machine. You can then run the playbook using the following command:
```
ansible-playbook playbook-name.yml
```

Please note that this playbook requires root privileges for most tasks. Therefore, you should either run it as a root user or a user with sudo permissions.

## Requirements

- Ansible 2.9 or higher
- Target hosts should be Linux machines with APT package manager

## Contributing

If you have suggestions for improving this playbook, please open an issue or submit a pull request.