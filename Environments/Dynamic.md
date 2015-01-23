<!SLIDE>
# Dynamic Environments

Environments configured generically using variables:

    @@@ ini
    [main]
      certname = puppet.example.com
      modulepath = /etc/puppet/environments/$environment/modules
      manifest = /etc/puppet/environments/$environment/manifests/site.pp
      server = puppet.example.com

    [agent]
      pluginsync = true
      environment = production

    [master]
      reports = tagmail

