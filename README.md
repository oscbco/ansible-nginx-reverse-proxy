Role Name
=========

Role setting up Nginx as a reverse proxy for our node.js server

Requirements
------------

Role Variables
--------------


Dependencies
------------

Example Playbook
----------------

    - hosts: servers
      roles:
        - {
            role: oscbco.nginx_reverse_proxy_domain,
            site_url: oscbco.me,
            appname: "{{ global_appname }}",
            template: "./server_dev.j2",
            certificate_file: "./oscbco.me.crt",
            privatekey_file: "./oscbco.me.pem"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
