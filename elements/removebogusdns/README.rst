==============
removebogusdns
==============

This element, Is a hack element which makes sure that resolv.conf is empty upon images creation. It has been noted that
rocky and centos images contained a dummy entry which created issues on image boot

More info can be found <https://opendev.org/openstack/diskimage-builder/src/branch/master/diskimage_builder/lib/common-functions#L376>

Environment Variables
---------------------

DIB_FINAL_RESOLV:
   :Required: Yes
   :Default: None
   :Description: The location of an empty resolv.conf.ORIG file on the Builder system which will be injected into the image
   :Example: ``DIB_FINAL_RESOLV=/etc/resolv.conf.ORIG ``
