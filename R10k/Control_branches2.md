<!SLIDE>
# Branches Become Environments

R10k will create an environment for each branch of the control repository.

    croddy@devbox $ git branch
      dev
      preprod
    * production
      test

After `r10k deploy environment -p`...

    /etc/puppet/environments
    ├── dev
    │   ├── dist
    │   │   ├── profiles
    │   │   └── roles
    │   ├── environment.conf
    │   ├── hieradata
    │   │   └── ...
    │   ├── manifests
    │   │   └── site.pp
    │   ├── modules
    │   │   ├── denyhosts
    │   │   ├── firewall
    │   │   ├── ngircd
    │   │   ├── stdlib
    │   │  ...
    │   └── Puppetfile
    │
    ├── preprod
    │   └── ...
    ├── production
    │   └── ...
    └── test
        └── ...

