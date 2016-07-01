# ER-wizard-OLSRd_V1
OLSRd (V1) Wizard for Ubiquiti EdgeMAX Devices supporting Wizards

    Works on EdgeRouter and EdgeRouter X / X-SFP (tested on System versions 1.7.0 and 1.8.0)

    known bugs:
    *) WebUI: feature wizard "TCP MSS clamping" hangs when feature wizard "OLSRd_V1" is added
    *) wizard.html: wrong position (10px lower than should be) of olsrd logo in mozilla firefox
    *) wizard-run: onlinecheck: fallback from ipv6 to ipv4 does not work because dns resolver prefers v6 (if ipv6 is configured)
    *) wizard-run: (if uncommenting auto-renaming wizard) after renaming wizard-dir, wizard still has wrong name in webif until user relogin
    *) wizard-run: olsrd6: skipping interfaces with site-local only v6 addresses (does not work with olsrd 0.6.6.2 ?)
    *) wizard-run: olsrd6: setting multicast does not work with olsrd 0.6.6.2
    updates:
    *) 05/2016 fixed wizard-run: enabled vlans are now correctly displayed as enabled
    *) 06/2016 fixed wizard-run: added architecture check for ER (mips) and ER-X (mipsel)
    feature requests in work:
    *) run olsrd on localhost with config setting "MainIp"
