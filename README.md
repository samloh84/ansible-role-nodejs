nodejs
=========

Ansible role for downloading Node.js binary or source archives to the control server, then extracting them to the target host.

Role Variables
--------------
Set the ```nodejs_version``` parameter to install other versions of Node.js

        nodejs_version: 6.7.0
        
Available versions:

    6.7.0
    5.12.0
    4.6.0
    0.12.16
    0.10.47

Set the ```prefix``` parameter to install somewhere other than ```opt/nodejs```

        prefix: "opt/nodejs"

Set the ```compile``` parameter to ```yes``` to compile Node.js from source

        compile: no
        
License
-------

MIT

Testing
-------
Run one of the following commands:

        ansible-playbook nodejs/tests/test.yml
        ansible-playbook --extra-vars "compile: true" nodejs/tests/test.yml

