ansible-cylance
=========

Cylance keeps your organization ahead of threat actors with AI-driven security tools that provide best-in-class detection, prevention, and response capabilities. Our highly trained specialists are available to augment your security staff or install our advanced solutions tailored to your exact needs. This ansible role installs and configures the agent required to communicate with client machines.

Requirements
------------
```bash
redhat_cylance_agent_filename: #redhat installer msi
windows_cylance_agent_filename: #windows installer msi
cylance_venue_id: #cylance venue id
cylance_proxy_id: #cylance proxy url
cylance_pid_id: #cylance pid id

```
Role Variables
--------------

```bash
None
```

Dependencies
------------
Acquire Installers
```bash
cylance.rpm - redhat installer package
cylance.msi - windows installer package
```

Example Playbook
----------------

```bash
    - hosts: servers
      roles:
         - ansible-cylance
```

License
-------

MIT

Author Information
------------------

Lance White - GSA/GEO
