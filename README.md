# ansible-mac-setup

<p align="center">
	<a href="https://github.com/msveinsson/ansible-mac-setup/actions/workflows/ansible-lint.yml"><img align="center" src="https://github.com/msveinsson/ansible-mac-setup/actions/workflows/ansible-lint.yml/badge.svg"/></a>
	<a href="https://img.shields.io/github/issues"><img align="center" src="https://img.shields.io/github/issues/msveinsson/ansible-mac-setup"/></a>
	<a href="https://github.com/msveinsson/ansible-mac-setup/commits/main"><img align="center" src="https://img.shields.io/github/commit-activity/m/msveinsson/ansible-mac-setup" alt="commit frequency"></a>
</p>

```sh
# Run all
ansible-playbook setup.yml --ask-become-pass

# Run using tags
ansible-playbook setup.yml --ask-become-pass

# Run with vault password
ansible-playbook --vault-password-file ~/private/ansible-vault/secret.mac.setup --ask-become-pass
```

Inventory file
```sh
[localhost]
"Macbook Pro" ansible_host=127.0.0.1  ansible_connection=local
```