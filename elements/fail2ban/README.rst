========
fail2ban
========

This element installs the fail2ban additional binary from the upstream repositories 
in the case of rocky linux, fail2ban lives in epel so the 'epel' element must also be included

In additiona, a compulsory jail.local is expected on the build system to be insterted in the final image

Environment Variables
---------------------

DIB_FAIL2BAN_CONF:
   :Required: Yes
   :Default: None
   :Description: The location of a fail2ban.conf file on the Builder system which will be injected into the image
   :Example: ``DIB\_FAIL2BAN\_CONF==~/home/jail.local``

