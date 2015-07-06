# Ansible Daemon Garden Role

[![Build Status](https://travis-ci.org/foomo/ansible-role-daemon-garden.png?branch=master)](https://travis-ci.org/foomo/ansible-role-daemon-garden)

> `daemon-garden` is an [ansible](http://www.ansible.com) role which:
>
> * installs daemon-garden

## Installation

Using `ansible-galaxy`:

```
$ ansible-galaxy install foomo.daemon-garden
```

Using `requirements.yml`:

```
- src: foomo.daemon-garden
```

Using `git`:

```
$ git clone https://github.com/foomo/ansible-daemon-garden.git foomo.daemon-garden
```

## Dependencies

* Ansible >= 1.9

## Variables

Here is a list of all the default variables for this role, which are also available in `defaults/main.yml`.

```
# package name (version)
daemon_garden_package: daemon-garden
```

## Handlers

These are the handlers that are defined in `handlers/main.yml`.

* `restart daemon-garden`

## Example playbook

```
- hosts: all
  sudo: yes
  roles:
    - foomo.daemon-garden
```

## Testing

```
$ git clone https://github.com/weareinteractive/ansible-daemon-garden.git
$ cd ansible-daemon-garden
$ vagrant up
```

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests and examples for any new or changed functionality.

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## License
Copyright (c) foomo under the LGPL 3.0 license.
