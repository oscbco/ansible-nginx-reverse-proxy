Role Name
=========

Role setting up Nginx as a reverse proxy for our Node.js server and static server for our /public folder

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
            appdir: "{{ global_appdir }}",
            site_url: oscbco.me,
            appport: "3000"
          }

License
-------

MIT

Author Information
------------------

oscbco.me
