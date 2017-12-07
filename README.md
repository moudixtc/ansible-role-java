Role Name: moudixtc.java
=========

Installs Java. Currently only [Zulu Java OpenJDK](https://www.azul.com/products/zulu-and-zulu-enterprise) is supported.

Requirements
------------

N/A

Role Variables
--------------

Refer to the [defaults](defaults/main.yml) and all the package manager and distribution specific variables in /vars directory.

Dependencies
------------

N/A

Example Playbook
----------------

To install an older version of zulu-8 on ubuntu. The package installed will be `zulu-8=8.23.0.3`, and it is Java `8u144`:

    - hosts: servers
      tasks:
        - include_role:
            name: moudixtc.java
          vars:
            java_version: '8.23.0.3'

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
