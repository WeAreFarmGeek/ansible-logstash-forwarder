Logstash-forwarder ansible role
===============================

Setup
-----

Use the SSL keys you generated for your logstash configuration ([see here for instructions on how to do that](https://github.com/johnhamelink/ansible-logstash)), and copy the .key and .crt files you generated into `roles/logstash-forwarder/files/certs`.

Copy `vars/global_vars.yml.sample` and customise it to suit your setup - it should be fairly self explanatory.

This ansible config installs a .deb generated from the logstash-forwarder sources. You can generate your own by following the instructions [here](https://github.com/elasticsearch/logstash-forwarder#building-it).

Installation
------------

### Logstash-forwarder:

`ansible-playbook logstash-forwarder.yml`

