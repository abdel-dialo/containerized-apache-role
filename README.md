containerized-apache-role
=========

Apache installation using docker

Requirements
------------

Centos 7

Role Variables
--------------

| name | type | description | mandatory |

| `external_port`         | int    | External port the httpd docker container                                           |   yes  |
                                                 
| `internal_port`         | int    | Internal port the httpd docker container                                           |   yes     |

| `system_user`           | string | The system user of remote nodes                                                    |   yes     |

| `template_file`         | string |template name use for the index.html file which will be mounted in the container  | yes |



Example Playbook 
----------------
See  [deploy containerized-apache-role](https://github.com/abdel-dialo/mini-projet-ansible)

```yaml

- name: "Apache installation using docker"
  hosts: your_hosts
  become: true
  roles:
    - containerized-apache-role


```



