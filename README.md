Ansible Bulldozer rebuild playbook
----------------------------------

The purpose of this playbook is to help me rebuild my workstations. There are a few prerequisets to using this playbook.

 * You must download the contents of this repo to your local system. The easiest way is with git and cloning it. If you choose to clone the repo then git must be installed before hand.
 * Ansible must be on the system. This can be installed from the repo, a git clone, or pip. The choice is yours.

Once you have the playbook run the following:

```Shell
ansible-playbook site.yml -K
```

This will prompt you for your password (for sudo) to use for package installs.

Feel free to use for your own purposes.
