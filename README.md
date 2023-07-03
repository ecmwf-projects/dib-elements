
# ECMWF Image Elements

This repository provides OpenStack `Diskimage Builder (DIB)
<https://github.com/openstack/diskimage-builder>` elements for the images build at ECMWF infrastructure

The list has been tested using python 3.6.8 and DIB 3.19.1 
on a centos stream 8 builder

## Elements

This repository provides the following DIB elements:

* ``fail2ban`` Installs fail2ban on the distro and inserts a custom fail2ban.conf file during creation
* ``locales``: Installs aditional locales when needed.
* ``centos-install-extra``: Additional binaries are required by users in EWC. (OBSOLETE)
* ``autoupdates``: Enables autoupdates from security repos for the images.
* ``prometheus-exporter``: Enables installation of the prometheus exporter from the Binaries built locally at ECMWF and hosted on nexus
* ``removebogusdns``: Removes the bogus DNS entry that is found in upstream rocky builds
