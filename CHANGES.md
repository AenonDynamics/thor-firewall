Changelog
===================================

## Branch 1..X ##

### 1.0.0 ###

* Added: support for multiple configuration files using `conf.d` style directory. Only used in case legacy `fw_fules.conf` doesn't exist!
* Added: help + version info
* Added: `systemd reload` triggers firewall restart
* Changed: iptables bin location (within `thor.conf`) to `/usr/sbin/iptables-nft`
* Changed: **License to Mozilla Public License 2.0 (MPL-2.0)**

## Prelimiary Release ##

### 0.3.0 ###
* Added: Show total firewall-rule count
* Changed: Invalid rules are skipped
* Changed: Removed ASLR kernel setting
* Bugfix: systemd doesn't wait for thor-firewall service completed

### 0.2.2 ###
* Initial Public Release