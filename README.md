cylance [![circleci](https://circleci.com/gh/GSA/ansible-cylance.svg?style=svg)](https://circleci.com/gh/GSA/ansible-cylance)
=========

This ansible role installs and configures the cylance agent required to communicate with client machines.

Requirements
------------

Required Packages
- cylance.rpm - redhat installer package
- cylance.msi - windows installer package

Role Variables
--------------

- redhat_cylance_agent_filename: #redhat installer msi
- windows_cylance_agent_filename: #windows installer msi
- cylance_venue_id: #cylance venue id
- cylance_proxy_id: #cylance proxy url
- cylance_pid_id: #cylance pid id

Dependencies
------------

None

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - ansible-cylance
```

Public domain
-------------

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
