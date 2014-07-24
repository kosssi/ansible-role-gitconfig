# ansible-role-gitconfig

[![Build Status](https://travis-ci.org/kosssi/ansible-role-gitconfig.svg?branch=master)](https://travis-ci.org/kosssi/ansible-role-gitconfig)

Ansible role to configure git.

## Role Defaults Variables

    git_config:
      <section>:
        <key>: <value>
    git_ignore:
      - ".vagrant"
      - ".DS_Store"

Example:

    git_config:
      user:
        name: Your Name
        email: your-email@exemple.org
      core:
        editor: vim
        excludesfile: "~/.gitexcludesfile"
      push:
        default: current
    git_ignore:
      - "*.log"
      - ".vagrant"

## Example Playbook

      roles:
        - { role: kosssi.gitconfig }

## Vagrant

If you have vagrant, you can test this role:

    cd tests
    vagrant up

## License

MIT
