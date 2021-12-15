vsftpd
=========

Install vsftpd

Requirements
------------

* RHEL-Based OS
* Python libs for SELinux

Role Variables
--------------

In defaults:

* anonymous_enable: yes
* upload_path: /var/ftp/pub/upload/
* ftp_path: /var/ftp/pub/
* local_enable: YES
* anon_root: /var/ftp/pub/upload
* no_anon_password: YES


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - name: Install vsftpd
      hosts: ftp

      roles:
        - role: vsftpd





