icingabeat
==========

Icingabeat Installer

!!! This is only suggested to be used in Lab environments!

Role Variables
--------------

    # Connect to the icinga2 API
    icingabeat_api_host: localhost
    icingabeat_api_port: 5665
    icingabeat_api_user: icinga
    icingabeat_api_password: icinga
    # by default the ssl certificate will be validated, which might is blocking the module from working in a lab environment
    icingabeat_api_ssl_verify: "true" # needs to be a string of "true" or "false"
    # connect to elasticsearch
    icingabeat_elasticsearch_host: localhost
    icingabeat_elasticsearch_port: 9200
    # still missing the authentification part

Example Playbook
----------------

    - hosts: icingabeat
      roles:
         - { role: andrelohmann.icingabeat }

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
