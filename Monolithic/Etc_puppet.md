<!SLIDE>
# Puppet Super Overmind Monolith
All of `/etc/puppet` as a repository:

    /etc/puppet/
    ├── environments
    │   ├── dev
    │   │   ├── hieradata
    │   │   ├── manifests
    │   │   └── modules
    │   │       └── ...
    │   ├── production
    │   │   ├── hieradata
    │   │   ├── manifests
    │   │   └── modules
    │   │       └── ...
    │  ...
    ├── manifests
    ├── modules
    │   └── ...
    ├── hiera.yaml
    ├── puppet.conf
    └── ssl
        ├── ca
        ├── certificate_requests
        ├── certs
        ├── private
        ├── private_keys
        └── public_keys

...`private_keys`???
