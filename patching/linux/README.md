# Weekly Patches Playbook for Linux

This Ansible playbook is designed to automate the process of updating and upgrading packages on Linux hosts. It performs the following tasks:

1. Updates the package lists for upgrades and new package installations.
2. Upgrades all the installed packages on the host.
3. Checks if the system requires a reboot after the upgrade.
4. If a reboot is required, it reboots the system.

## Usage

To run this playbook, you need to have Ansible installed on your machine. You can then run the playbook using the following command:
```
ansible-playbook weekly-patches.yml
```

When you run the playbook, it will first prompt you to enter the target hosts and the connection type. You can enter the IP address or hostname of your Linux machine and the appropriate connection type (usually `ssh`).

Please note that this playbook requires root privileges for most tasks. Therefore, you should either run it as a root user or a user with sudo permissions.

## Requirements

- Ansible 2.9 or higher
- Target hosts should be Linux machines with APT package manager

## Contributing

If you have suggestions for improving this playbook, please open an issue or submit a pull request.

Happy patching!