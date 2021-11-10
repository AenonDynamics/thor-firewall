thor-firewall
========================================

an iptables firewall loader initialized via systemd

```raw
  _____ _   _  ___  ____       _____ _                        _ _
 |_   _| | | |/ _ \|  _ \     |  ___(_)_ __ _____      ____ _| | |
   | | | |_| | | | | |_) |____| |_  | | '__/ _ \ \ /\ / / _` | | |
   | | |  _  | |_| |  _ <_____|  _| | | | |  __/\ V  V / (_| | | |
   |_| |_| |_|\___/|_| \_\    |_|   |_|_|  \___| \_/\_/ \__,_|_|_|
```

## Features ##

* Load iptable rulesets via text files
* Split rulesets into multiple files
* Host or Router operation mode (forwarding enabled)
* sysctl routing tweaks
* Display current iptable ruleset
* well documented sourcecode (line wise)
* full systemd integration
* Currently limited to ipv4

## Usage ##

```
Usage: thor-firewall <command> [args...]

Options:
    -h,--help               Displays this help
    -v,--version            Displays version

Commands:
    start                   Initialize firewall rules/tables/chains
    stop                    Flush all iptables chains/rules
    restart                 Reload/Initialize firewall rules/tables/chains
    open                    WARNING: Dropping all Firewall+NAT Rules and set system to ACCEPT ALL
    status                  Show all configures rules/tables/chains
```



## Docs ##

* [OpenWRT integration](docs/openwrt.md)

## Environments ##

Tested with:

* Debian Jessie/Stretch/Buster/Bullseye
* OpenWRT 18/19

## Contribution ##

The **.deb** package is automatically generated via a **Continuous Delivery Pipeline** - please do not build packages manually!

## License ##
THOR-FIREWALL is OpenSource and licensed under the Terms of [Mozilla Public License 2.0 (MPL-2.0)](http://opensource.org/licenses/MPL-2.0) - your're welcome to contribute