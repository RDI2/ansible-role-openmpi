Ansible Role - openmpi
======================

This role installs openmpi into `/opt/openmpi/{{ openmpi_version }}`.

Platforms
---------

CentOS 6.7 is the only platform that is supported and tested so far.

Default Variables
-----------------

- openmpi_version: `1.10.1`
- openmpi_url: `http://www.open-mpi.org/software/ompi/v1.10/downloads/openmpi-{{ openmpi_version }}.tar.bz2`
- openmpi_prefix: `/opt/openmpi/{{ openmpi_version }}`

Example Playbook
----------------

Include the role like this:

```yaml
- hosts: servers
  roles:
     - { role: rdi2sys.openmpi }
```

License
-------

MIT License.

Author
------

- Koji Tanaka - RDI2
