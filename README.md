# wpa_supplicant_example

This is a small sample of a wpa_supplicant configuration. 

## Networks
To explain the file a little bit, you can specify as many networks as needed 
and also on them some may require additional configuration options or not,
depending on your network safety protocols.

## Setting a group
You need to specify the group which can interact with the wpa_supplicant
daemon, groups such as sudoers for example.

## Network Wildcard
The very last network specified acts as a wildcard, it will connect to networks which 
require authentication (public).

## Priority
The priority is inversed, the higher the value, the more priority it gets
when establishing a connection. 

## Why does this not automatically connect to the wifi
This file does not hotplug the wifi, that needs
to be configured on the _/etc/networks/interfaces_ file.

## Sources:
* https://w1.fi/cgit/hostap/plain/wpa_supplicant/wpa_supplicant.conf
