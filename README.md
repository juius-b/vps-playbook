# Virtual Private Server (VPS)

This project contains everything that concerns my VPS.

## Getting started

Copy `group_vars/all/vars.yml` to `group_vars/all/vault_vars.yml`. At least fill in the variables that are commented with "mandatory". As these almost certainly contain sensitive information, use ansible-vault to encrypt and edit the file.

## Installation

1. Run `ansible-playbook -i inventory main.yml`.

Keep in mind that a non-root user gets created during execution. Rerunning the playbook might need adjustment in the inventory file, your SSH config or specifying the remote user via the option `-u REMOTE_USER`.
