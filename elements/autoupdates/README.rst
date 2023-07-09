===========
autoupdates
===========

This element will configure Both ubuntu and rocky images to have enabled automatic updates from security repos. For ubuntu based images it is based on unuattended-upgrades and for rocky on dnf-automatic.

Environment Variables
---------------------

DIB_APT_UPDATES_CONF
   :Required: Yes 
   :Default: None
   :Description: The location of a default 50unattended-upgrades file on the builder Filesystem which will be injected into the image
   :Example: ``DIB_APT_UPDATES_CONF=/home/50unattended-upgrades``
