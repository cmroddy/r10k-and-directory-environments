<!SLIDE>
# Directory Environments
Set `basemodulepath` and `environmentpath` in `puppet.conf`:

    @@@ ini
    [main]
      certname = puppet.example.com
      basemodulepath = /etc/puppet/modules
      environmentpath = /etc/puppet/environments
      server = puppet.example.com

    [agent]
      pluginsync = true
      environment = production

    [master]
      reports = tagmail

Set `modulepath` and manifest in `environment.conf`:

    @@@ ini
    modulepath = modules:$basemodulepath

All manifests in `manifests` will be loaded (by default).
