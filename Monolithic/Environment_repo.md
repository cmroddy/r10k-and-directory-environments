<!SLIDE>
# Environment Repository

Each branch as the contents of a single environment:

    /etc/puppet/environments/production
    ├── hieradata
    ├── manifests
    │   └── site.pp
    └── modules
        ├── concat
        ├── denyhosts
        ├── firewall
        ├── git
        ├── inifile
        ├── ngircd
        ├── profiles
        ├── roles
        ├── stdlib
        ├── thttpd
        └── ...
