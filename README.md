Role Name
=========

Managing the Red Hat EPEL repository.

Requirements
------------

No requirements.

Role Variables
--------------

EPEL Repo package url refers to the url of epel-release-latest-X.noarch.rpm where X is replaced by the distribution
major release number. defaults/main.yml

```
epel_repo_pkg_url: "https://dl.fedoraproject.org/pub/epel/epel-release-latest-{{ ansible_distribution_major_version }}.noarch.rpm"
```

EPEL Repo GPG key url refers to the url of the GPG key used to sign the epel-release-latest-X.noarch.rpm where X is
replaced by the distribution major release number. defaults/main.yml

```
epel_repo_gpg_key_url: "https://dl.fedoraproject.org/pub/epel/RPM-GPG-KEY-EPEL-{{ ansible_distribution_major_version }}"
```

Dependencies
------------

No dependencies.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: wiredobjects.epel }

License
-------

Apache

Author Information
------------------

refnode
