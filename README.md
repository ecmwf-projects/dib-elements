
# ECMWF Image Elements

This repository provides OpenStack `Diskimage Builder (DIB)  <https://github.com/openstack/diskimage-builder>` elements for the images build at ECMWF infrastructure for CCI.

The list has been tested using python 3.6.8, DIB 3.19.1 on a centos stream 8 builder to build centos7,centos8-stream/ubuntu/debian/rocky images.

## Elements

This repository provides the following DIB elements:

* ``locales``: Installs aditional locales when needed in rocky and centos.
* ``prometheus-exporter``: Enables installation of the prometheus exporter from the binaries built locally at ECMWF and hosted on nexus.
* ``removebogusdns``: Removes the bogus DNS entry that is found in upstream rocky builds.
* ``rocky-install-extra``: Enables installation of additional binaries on rocky distributions, as requested by ECMWF users.
* ``ubuntu-install-extra``: Additional binaries are required by users in EWC for ubuntu.
* ``centos-install-extra``: Additional binaries are required by users in EWC for centos. (OBSOLETE)
