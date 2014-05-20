Ansible Bulldozer rebuild playbook
----------------------------------

The purpose of this playbook is to help me rebuild my workstations. There are a few prerequisets to using this playbook.

 * You must download the contents of this repo to your local system. The easiest way is with git and cloning it. If you choose to clone the repo then git must be installed before hand.
 * Ansible must be on the system. This can be installed from the repo, a git clone, or pip. The choice is yours.

Set up the Ansible host file to be able to connect to the localhost in /etc/ansible/hosts. Just replace <hostname> with your systems name.

```Shell
[localhost]
<hostname> ansible_connection=local
```

Once you have the playbook run the following:

```Shell
ansible-playbook site.yml -K --ask-vault-pass
```

This will prompt you for your password (for sudo) to use for package installs. You will also be prompted for your vault password for encrypted files found in host_vars.

Feel free to use for your own purposes.
