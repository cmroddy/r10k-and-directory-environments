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

(Legacy dynamic environments work, too)
