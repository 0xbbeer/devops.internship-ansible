Apache
=========

Install Apache

Requirements
------------

* RHEL-Based OS
* Debian-Based OS

Role Variables
--------------

In defaults:

* apache_packages_state: present
* apache_restart_state: restarted
* apache_state: started
* apache_enabled: true
* apache_server_admin: admin@example.com
* apache_port: 80

In vars:

- Rhel:
  
  * apache_service: httpd
  * apache_daemon: httpd
  * apache_package: httpd

- Deb:
  * apache_service: apache2
  * apache_daemon: apache2
  * apache_package: apache2

Dependencies
------------

-

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - name: Install Apache
      hosts: webservers

      roles:
        - role: apache

