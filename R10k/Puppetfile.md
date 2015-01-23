<!SLIDE>
# Puppetfile #

The `Puppetfile` lists the desired modules and their versions.

    # Modules from the Forge
    mod 'puppetlabs/firewall','1.1.3'
    mod 'puppetlabs/stdlib','4.3.2'
    mod 'puppetlabs/vcsrepo','1.1.0'

    # Modules from Git repositories
    mod 'denyhosts',
      :git => 'git@github.com:cmroddy/puppetlabs-denyhosts.git',
      :ref => '3403309a'

    mod 'ngircd',
      :git => 'git@github.com:cmroddy/puppet-ngircd.git',
      :ref => 'master'

    mod 'thttpd',
      :git => 'git@github.com:cmroddy/puppet-sthttpd.git',
      :ref => 'v1.2.3'

