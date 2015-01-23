<!SLIDE>
# Per-Environment Hiera data

`$environment` is interpolated in `hiera.yaml`.

    ---
    :backends:
      - yaml

    :hierarchy:
      - nodes/%{clientcert}
      - datacenters/%{datacenter}
      - platforms/%{operatingsystem}-%{operatingsystemrelease}
      - platforms/%{operatingsystem}
      - common

    :yaml:
      :datadir: /etc/puppet/environments/%{environment}/hieradata

