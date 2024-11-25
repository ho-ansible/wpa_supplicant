# Ansible role: `wpa_supplicant`
Wi-Fi client config.
This only configures the wifi link; DHCP etc. is handled separately by systemd-networkd, dhclient, et al.

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `wifi_iface` (default: wlan0): network interface bound to wireless NIC
+ `wifi_ssid` (default: `MY_SSID`): wifi ESSID to connect to
+ `wifi_passwd` (default: `MY_PASSWD`): plaintext passphrase for given ESSID

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run prior to removing host from inventory group.

## Dependencies
None

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
