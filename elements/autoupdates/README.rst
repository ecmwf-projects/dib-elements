===========
autoupdates
===========

This element will configure Both ubuntu and rocky images to have enabled automatic updates from security repos. For ubuntu based images it is based on unuattended-upgrades and for rocky on dnf-automatic.

Environment Variables
---------------------

DIB_APT_UPDATES_CONF
   :Required: Yes for the Debian Family
   :Default: None
   :Description: The location of a custom 50unattended-upgrades file on the builder which will be injected into the image
   :Example: ``DIB_APT_UPDATES_CONF=/home/50unattended-upgrades``

DIB_ROCKY_UPDATES_CONF
   :Required: Yes for the Redhat Family
   :Default: None
   :Description: The location of a custom automatic.conf file on the builder which will be injected into the image
   :Example: ``DIB_ROCKY_UPDATES_CONF=/home/automatic.conf``
