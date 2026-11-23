# Board Profiles

The supported target is the **ESP32-S31-Function-CoreBoard-1**.

`defaults.conf` contains settings shared by all profiles. `production.conf`
contains the deployable station-mode port configuration without stress-test
applications. `softap.conf` enables Wi-Fi SoftAP mode (`wlan0`) with a DHCP
server. `sta_softap.conf` enables concurrent Wi-Fi Station (`wlan0`) and
SoftAP (`wlan1`) coexistence with a DHCP server and IPv4 forwarding/NAT.
`validation.conf` extends production with the applications and diagnostics
required by the bounded hardware regression suite.

NuttX board defconfigs remain compatibility entry points. The root `build.sh`
and these profiles are the reproducible integration entry points.
