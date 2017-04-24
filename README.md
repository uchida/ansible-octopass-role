uchida.octopass
===============

ansible role to install [octopass](https://github.com/linyows/octopass),
management linux user and authentication with the organization/team on Github.

Role Variables
--------------

- `octopass_token`: required
- `octopass_organization`: required
- `octopass_team`: required
- `octopass_endpoint`: optional
- `octopass_group`: optional
- `octopass_home`: optional
- `octopass_shell`: optional
- `octopass_uidstarts`: optional
- `octopass_gid`: optional
- `octopass_cache`: optional
- `octopass_syslog`: optional
- `octopass_sharedusers`: optional

Example Playbook
----------------

```
- hosts: servers
  become: yes
  roles:
    - role: uchida.octopass
      octopass_token: XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX
      octopass_organization: your organization
      octopass_team: your team
```

License
-------

Dedicated to [![CC0 public domain](http://i.creativecommons.org/p/zero/1.0/80x15.png "CC0 public domain")](https://creativecommons.org/publicdomain/zero/1.0/).
No rights reserved.
