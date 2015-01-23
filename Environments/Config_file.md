<!SLIDE>
# Config-File Environments
Each environment configured explicitly in `puppet.conf`:

    @@@ ini
    [main]
      certname = puppet.example.com
      modulepath = /etc/puppet/modules
      manifest = /etc/puppet/manifests/site.pp
      server = puppet.example.com

    [agent]
      pluginsync = true
      environment = production

    [master]
      reports = tagmail

    [dev]
      modulepath = /etc/puppet/environments/dev/modules
      manifest = /etc/puppet/environments/dev/site.pp

    [test]
      modulepath = /etc/puppet/environments/test/modules
      manifest = /etc/puppet/environments/test/site.pp

    [preprod]
      modulepath = /etc/puppet/environments/preprod/modules
      manifest = /etc/puppet/environments/preprod/site.pp
