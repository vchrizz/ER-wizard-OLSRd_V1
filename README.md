# ER-wizard-OLSRd_V1
OLSRd (V1) Wizard for Ubiquiti EdgeMAX Devices supporting Wizards

    Github repository: https://github.com/vchrizz/ER-wizard-OLSRd_V1/

    Works on all EdgeRouter and EdgePoint Devices (system version 1.7.0+)

    known bugs:
    *) WebUI: feature wizard "TCP MSS clamping" hangs when feature wizard "OLSRd_V1" is added
    *) wizard.html: wrong position (10px lower than should be) of olsrd logo in mozilla firefox
    *) wizard-run: onlinecheck: fallback from ipv6 to ipv4 does not work because dns resolver prefers v6 (if ipv6 is configured)
    *) old olsrd for ipv6 was installed as "olsrdv6", new version with "olsrd6" --> fix this by firmware-upgrade!
    updates:
    *) 05/2016 fixed wizard-run: enabled vlans are now correctly displayed as enabled
    *) 06/2016 fixed wizard-run: added architecture check for ER (mips) and ER-X (mipsel)
    *) 10/2016 fixed wizard-run: added olsrd 0.6.6.2-1 packages in base64 format for offline installation
    *) 10/2016 fixed wizard-run: updated olsrd packages to version 0.9.0.3-1 for mipsel architecture
    *) 10/2016 fixed wizard-run: updated olsrd packages to version 0.9.0.3-1 for mips architecture
    *) 10/2016 fixed wizard-run: added check if latest version is installed from available packages on disk
    *) 02/2017 CPO: fixed olsrd_setup.sh arch check, patch existing installations, remove prev.version install-scripts
    *) 02/2017 CPO: fix migration from old to new version related to old default/config files (mentioned in /etc/default/olsrd)
    *) 02/2017 CPO: fix migration from very-old to new version related configfiles in /etc/olsrd instead of /config/user-data)  
    *) 02/2017 CPO: fix olsrd6.conf for using LinkQualityMult - param IpVersion is needed before LQ factors to parse IPv6 entries
    *) 02/2017 CPO: feature - restart olsrd for IPv4 and IPv6 individually
  
