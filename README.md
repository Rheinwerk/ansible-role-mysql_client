Install Percona MySQL Client Packages
=========

This role can be used to install the Percona MySQL Client Tools.

[![Build Status](https://travis-ci.org/Rheinwerk/ansible-role-mysql_client.svg?branch=master)](https://travis-ci.org/Rheinwerk/ansible-role-mysql_client)

Requirements
------------

None.


Role Variables
--------------

There is one main variable that drives this role: `_mysql_client`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_mysql_client` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        MYSQL_CLIENT
          ...
      roles:
         - { role: mysql_client, tags: [ 'mysql_client' ], _mysql_client: "{{ MYSQL_CLIENT }}" }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

