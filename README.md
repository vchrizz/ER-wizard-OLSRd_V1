# ER-wizard-OLSRd_V1
OLSRd (V1) Wizard for Ubiquiti EdgeMAX Devices supporting Wizards

branch to refurbish the UI and to solve install issues on EdgeOS v2.0.0
and to prepare new release including 0.9.7

what to work on:
* [done] repacked olsrd packages 0.9.6.2
* [done] support clean dpkg installation for EdgeOS v2.0
* [done] fix paths to plugins (dynamically?)
* [done] write a config migration script to move from "old" config style to "new" without dead freight
* [done] new etc-init.d scripts including logging and watchdog handling
* [done] new config sections, one for each activated interface
* [done] remove interfaces from startup-parameters
* [done] get rid of old code and patches, that are no longer needed.
* [done] HNAs and LQs into default interface section
* [done] add olsr-after-ntp.sh to restart olsrd after cold-boot and ntp-sync
* [done] UI: one line for each hna entry and subnet (add and remove buttons), check syntax/values
* [done] UI: one line for each LQ entry (add and remove buttons), check syntax and values
* [done] UI: select mode (mesh, silent, ether) for each interface individually
* [done] UI: manage default-lq for each interface individually
* [done] UI: configure "main ip" for routers having multiple public IPs
* [done] add RtProto, RtTable, RtTableDefault, MainIp, Weight to config-migration scripts
* [done] tune default parameters of info-plugins (especially httpinfo plugin allowed hosts/subnets)
* [done] establish "links" script in /usr/bin/local, as of this script: https://gist.githubusercontent.com/pocki80/eeea81945111ac14b937bd46b83412d2
* [dismissed] configure AutoDetectChanges for InterfaceDefaults
* [dismissed] handle second+ IPs of an olsr interface as HNA automatically?
* [dismissed] activate httpinfo, watchdog on install "by default"?
* [dismissed] save important data to "custom-attributes" in EdgeOS configuration?
* UI: paramsection for infoplugins (at least for httpinfo subnets/hosts)
* improve handling of bridges with ebtables! only block what is really needed (i.e. use --logical-in)
