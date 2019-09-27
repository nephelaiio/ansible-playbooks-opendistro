# nephelaiio.playbooks-upgrade

[![Build Status](https://travis-ci.org/nephelaiio/ansible-playbooks-upgrade.svg?branch=master)](https://travis-ci.org/nephelaiio/ansible-playbooks-upgrade)

Ansible playbook to upgrade OS packages.

## Playbook descriptions

The following lists the group targets and descriptions for every playbook

| playbook          | description                                                             | target                   |
| ---               | ---                                                                     | ---                      |
| elasticsearch.yml | install elasticsearch with openditro plugins using standalone procedure | opendistro_elasticsearch |

## Playbook variables

The following parameters are available/required for playbook invocation

### [elasticsearch.yml](local.yml):
| required | variable                        | description                                             | default |
| ---      | ---                             | ---                                                     | ---     |
| no       | opendistro_release              | elasticsearch version                                   | 1.2.0   |

## Dependencies

This playbook has the following git submodule dependencies:

* [plugins/mitogen](https://github.com/dw/mitogen)

## Example Invocation

```
git checkout https://galaxy.ansible.com/nephelaiio/ansible-playbooks-upgrade upgrade
ansible-playbook -i inventory/ upgrade/upgrade.yml
```

## License

This project is licensed under the terms of the [MIT License](/LICENSE)
