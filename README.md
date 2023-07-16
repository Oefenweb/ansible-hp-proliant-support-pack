## hp-proliant-support-pack

[![CI](https://github.com/Oefenweb/ansible-hp-proliant-support-pack/workflows/CI/badge.svg)](https://github.com/Oefenweb/ansible-hp-proliant-support-pack/actions?query=workflow%3ACI)
[![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-hp--proliant--support--pack-blue.svg)](https://galaxy.ansible.com/Oefenweb/hp_proliant_support_pack)

Install HP Proliant support pack.

#### Requirements

* `software-properties-common` (will be installed)
* `dirmngr` (will be installed)

#### Variables

None

* `hp_proliant_support_pack_install`: [default: see `defaults/main.yml`]: Packages to install
* `hp_proliant_support_pack_install.{n}.name`: [required]: Package name
* `hp_proliant_support_pack_install.{n}.codename`: [optional, default: `ansible_distribution_release`]: Codename of target release to use
* `hp_proliant_support_pack_install.{n}.state`: [optional, default: `latest`]: Indicates the desired package state

* `hp_proliant_support_pack_repository_version`: [default: `current`]: Repository version to use (e.g. `12.40`)

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
