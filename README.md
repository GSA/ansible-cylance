cylance [![circleci](https://circleci.com/gh/GSA/ansible-cylance.svg?style=svg)](https://circleci.com/gh/GSA/ansible-cylance)
=========

This ansible role installs and configures the cylance agent required to communicate with client machines.

Requirements
------------

Required Packages (this role requires access to the following packages/installers via an external repository)
- cylance.rpm - redhat installer package
- cylance.msi - windows installer package

Role Variables
--------------

### Universal

| Variable | Default | Purpose |
| ------ | ------ | ------ |
| cylance_venue_id | "" | cylance venue id |
| cylance_pid_id | "" | cylance key |

### Windows

| Variable | Default | Purpose |
| ------ | ------ | ------ |
| windows_cylance_agent_path | "C:\\Program Files\\Cylance\\Desktop" | default windows install directory |
| windows_cylance_agent_url | "" | windows installer msi |
| windows_cylance_product_id | "" | windows product_id |
| windows_agent_log | "C:\Temp\Logs" | default agent windows log directory |

### Redhat

| Variable | Default | Purpose |
| ------ | ------ | ------ |
| redhat_cylance_agent_path | "/opt/Cylance/desktop" | default redhat install directory |
| redhat_cylance_agent_url | "" | redhat installer rpm |

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - cylance
```

Public domain
-------------

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
