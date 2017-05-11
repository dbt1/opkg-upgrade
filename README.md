# opkg-upgrade
List and install OpenWRT / LEDE opkg upgradable packages
 
Little ash app for easier opkg package upgrades.
You should check for config conflicts after upgrades!
  
### Help example:
```
# ./opkg-upgrade.sh -h

Simple OPKG Updater v0.1.2

Usage: opkg-upgrade.sh [-n,-f]

Options:
  -V, --version           Show program name and version and exits
  -h, --help              Show this help screen and exits
  -n, --no-opkg-update    Skip opkg update at the beginning,
                          may not find packages if not up to date
  -f, --force             Do not ask for confirmation,
                          will update everything available

Notes:
  Parameters should not be grouped.
  You must pass each parameter on its own.
  The order is irrelevant.

Examples:
  opkg-upgrade.sh -nf     # INVALID PARAMETER
  opkg-upgrade.sh -n -f   # VALID PARAMETERS
```
### Example run:
```
# ./opkg-upgrade.sh

Simple OPKG Updater v0.1.2

Done | Updating package lists
Done | Getting upgradable packages list

Packages available for upgrade: 23

luci-app-statistics - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-adblock - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-lib-ip - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-samba - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-theme-bootstrap - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-qos - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-firewall - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-diag-core - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-proto-ppp - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-mod-admin-full - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-base - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-commands - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-vnstat - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-proto-ipv6 - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-wol - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-upnp - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-minidlna - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-lib-nixio - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-lib-jsonc - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-p910nd - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-transmission - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1
luci-app-openvpn - git-17.126.47277-596f476-1 - git-17.129.29271-6467df3-1

Proceed with upgrade? (Y/y to proceed) y

.... | Upgrading packages

Upgrading luci-app-statistics on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-statistics_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-adblock on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-adblock_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-lib-ip on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-lib-ip_git-17.129.29271-6467df3-1_mipsel_74kc.ipk
Upgrading luci-app-samba on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-samba_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-theme-bootstrap on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-theme-bootstrap_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-qos on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-qos_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-firewall on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-firewall_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-diag-core on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-diag-core_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-proto-ppp on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-proto-ppp_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-mod-admin-full on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-mod-admin-full_git-17.129.29271-6467df3-1_mipsel_74kc.ipk
Upgrading luci-base on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-base_git-17.129.29271-6467df3-1_mipsel_74kc.ipk
Upgrading luci-app-commands on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-commands_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-vnstat on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-vnstat_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-proto-ipv6 on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-proto-ipv6_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-wol on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-wol_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-upnp on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-upnp_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-minidlna on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-minidlna_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-lib-nixio on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-lib-nixio_git-17.129.29271-6467df3-1_mipsel_74kc.ipk
Upgrading luci-lib-jsonc on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-lib-jsonc_git-17.129.29271-6467df3-1_mipsel_74kc.ipk
Upgrading luci-app-p910nd on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-p910nd_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-transmission on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-transmission_git-17.129.29271-6467df3-1_all.ipk
Upgrading luci-app-openvpn on root from git-17.126.47277-596f476-1 to git-17.129.29271-6467df3-1...
Downloading http://downloads.lede-project.org/releases/17.01.1/packages/mipsel_74kc/luci/luci-app-openvpn_git-17.129.29271-6467df3-1_all.ipk
Configuring luci-app-statistics.
Configuring luci-lib-jsonc.
Configuring luci-app-adblock.
Configuring luci-lib-nixio.
Configuring luci-lib-ip.
Configuring luci-base.
Configuring luci-mod-admin-full.
Configuring luci-app-firewall.
Configuring luci-app-samba.
Configuring luci-theme-bootstrap.
Configuring luci-app-qos.
Configuring luci-app-diag-core.
Configuring luci-proto-ppp.
Configuring luci-app-commands.
Configuring luci-app-vnstat.
Configuring luci-proto-ipv6.
Configuring luci-app-wol.
Configuring luci-app-upnp.
Configuring luci-app-minidlna.
Configuring luci-app-p910nd.
Configuring luci.
Configuring luci-app-transmission.
Configuring luci-app-openvpn.
Collected errors:
 * resolve_conffiles: Existing conffile /etc/config/luci_statistics is different from the conffile in the new package. The new conffile will be placed at /etc/config/luci_statistics-opkg.
 * resolve_conffiles: Existing conffile /etc/config/luci is different from the conffile in the new package. The new conffile will be placed at /etc/config/luci-opkg.

Done | Upgrade finished

Please check for config file conflicts!
  
```
### When all up-to-date:
```
# ./opkg-upgrade.sh -f -n

Simple OPKG Updater v0.1.2

Done | Ignoring package lists update
Done | Getting upgradable packages list

No packages to install!
```