<!SLIDE>
# Configure R10k

R10k needs to know how to find the control repository.

    #/etc/r10k.yaml
    ---
    :cachedir: /var/cache/r10k
    :sources:
      puppet:
        basedir: /etc/puppet/environments
        remote: git@github.com:cmroddy/example-control.git

The user running R10k will usually need SSH keys.
