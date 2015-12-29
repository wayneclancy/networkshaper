Overview
--------
OpenWRT package to allow you to emulate diffrent types of network connections. Comes with a very simple web interface 
to control network profiles.
Based around slow (https://gist.github.com/denilsonsa/5176e1c9b6a119594ce0) and slightly modifed to work with ash on OpenWRT devices.


UI is accesable via http://$ROUTER_IP:8080

Building
--------
type 'make' in the root directory. This will create a .ipk file in ./build that should install on your openWRT device.

Installing
----------
run 
```opkg install https://raw.githubusercontent.com/wayneclancy/networkshaper/master/dist/networkshaper-f9164c3.ipk```

Alternativly copy ipk over to the the router via your prefered method and run 
```opkg install /$PATH_TO_IPK```

Assumptions
-----------
This only works if eth0 (WAN) port is being nated to LAN and Wifi interfaces.

Notes
------
This has only been tested on a TP-link WR710N (ver2.1) but should work on *most* hardware. 

Todo
----


