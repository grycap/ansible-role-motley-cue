[![License](https://img.shields.io/badge/license-Apache%202-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
[![CI](https://github.com/grycap/ansible-role-motley-cue/workflows/CI/badge.svg)](https://github.com/grycap/ansible-role-motley-cue/actions?query=workflow%3ACI)

# Motley-cue Role

This ansible role installs the [motley-cue](https://motley-cue.readthedocs.io/) software.
The github repository of the motley-cue is [here](https://github.com/dianagudu/motley_cue).

## Example Playbook

This an example of how to install this role:

    - hosts: server
      roles:
      - { role: 'grycap.motley-cue', ssh_oidc_my_vo: true, ssh_oidc_other_vos: 'vo_name' }

And then execute it with:

    ansible-playbook --extra-vars ACCESS_TOKEN=$(oidc-token <account>) playbook.yaml

To get the `oidc-token` command working please check [ssh-oidc](https://github.com/EOSC-synergy/ssh-oidc)

# Contributing to the role

In order to keep the code clean, pushing changes to the master branch has been disabled. If you want to contribute, you have to create a branch, upload your changes and then create a pull request.
Thanks
