# wpa_supplicant_example

This is a small sample of a wpa_supplicant configuration. 
To explain the file a little bit, you can specify as many networks as needed 
and also on them some may require additional configuration options or not,
depending on your network safety protocols.
Also, you need to specify the group which can interact with the wpa_supplicant
daemon, groups such as sudoers for example. Next, the last network specified
acts as a wildcard, it will connect to networks which require authentication (public).
Finally, the priority is inversed, the higher the value, the more priority it gets
when establishing a connection. Also this file does not hotplug the wifi, that needs
to be configure on the /etc/networks/interfaces file.

More info at: https://w1.fi/cgit/hostap/plain/wpa_supplicant/wpa_supplicant.conf
