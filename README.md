Role Name
=========

Role to set up a OpenVPN client and (optionally) a set of root certificates.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
    - vars:
        open_vpn_connection:
        - name: example
        - username: euser
        - vpn_cert_zip: ~/Files/vpn_Example_User.zip
        - only_for:
          - example.com
          - example.io
        certificate_urls:
        - http://pki.example.com/Example-Root-CA-v01.crt
        - http://pki.example.com/Example-Company-CA-v01.crt
        - http://pki.example.com/Example-Universal-Issuing-CA-v01.crt
      roles:
         - role: baztian.openvpn_client

License
-------

GPLv3
