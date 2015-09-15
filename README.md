# ansible-playbook-topbeat
An ansible playbook to install topbeat (https://www.elastic.co/downloads/beats/topbeat) on a debian/ubuntu machine

## Getting started
Add your hosts to the `hosts` file.

Set the variables in `playbook.yml`:

`packagename:` the name of the topbeat package you want to install. (e.g. topbeat_1.0.0-beta3_amd64.deb)
 
`es_host:` the name/ip of the elasticsearch host you want to use (e.g. 127.0.0.1)
 
`es_port:` the port of your elasticsearch host (e.g. 9200)

## Run the playbook
`ansible-playbook -i hosts ./playbook.yml`
