## hp-proliant-support-pack

[![Build Status](https://travis-ci.org/Oefenweb/ansible-hp-proliant-support-pack.svg?branch=master)](https://travis-ci.org/Oefenweb/ansible-hp-proliant-support-pack) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-hp--proliant--support--pack-blue.svg)](https://galaxy.ansible.com/Oefenweb/hp-proliant-support-pack)

Install HP Proliant support pack.

#### Requirements

None

#### Variables

None

* `hp_proliant_support_pack_install`: [default: see `defaults/main.yml`]: Packages to install
* `hp_proliant_support_pack_install.{n}.name`: [required]: Package name
* `hp_proliant_support_pack_install.{n}.codename`: [optional, default: `ansible_lsb.codename`]: Codename of target release to use
* `hp_proliant_support_pack_install.{n}.state`: [optional, default: `latest`]: Indicates the desired package state

## Dependencies

None

#### Example

```yaml
---
- hosts: all
  roles:
    - hp-proliant-support-pack
```

#### License

MIT

#### Author Information

* Mark van Driel
* Mischa ter Smitten

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Oefenweb/ansible-hp-proliant-support-pack/issues)!
