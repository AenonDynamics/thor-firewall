OpenWRT
=============================

The thor-firewall loader can also be used on an [OpenWRT](https://openwrt.org) based environment

## File Locations ##

Copy the files to their default locations:

* /sbin/thor-firewall
* /etc/thor-firewall/fw_rules.conf
* /etc/thor-firewall/thor.conf

## RC.d Startup ##

To start thor-firewall via rc.d (also accessable via UCI) just create a [init script](https://oldwiki.archive.openwrt.org/doc/techref/initscripts) which invokes the loader:

File: `/etc/init.d/thor_firewall` - Mode `0755`

```bash
#!/bin/sh /etc/rc.common
# THOR FIREWALL INIT
 
START=15
STOP=15
 
start() {        
     /sbin/thor-firewall start
}

restart() {
     /sbin/thor-firewall start
}
```