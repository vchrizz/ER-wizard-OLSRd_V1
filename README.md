# ER-wizard-OLSRd_V1
OLSRd (V1) Wizard for Ubiquiti EdgeMAX Devices supporting Wizards

branch to prepare new release including 0.9.7

what to work on:
* new olsrd packages
* fix paths to plugins (dynamically?)
* improve handling of bridges with ebtables! only block what is really needed (i.e. use --logical-in)
* tune default parameters of info-plugins (especialle httpinfo plugin allowed hosts/subnets)
* write a config migration script to move from "old" config style to "new" without dead freight
* new etc-init.d scripts including logging and watchdog handling
* new config sections, one for each activated interface
* remove interfaces from startup-parameters
* activate httpinfo, watchdog on install "by default"?
* HNAs and LQs into default interface section
* UI: one line for each hna entry and subnet (add and remove buttons), check syntax/values
* UI: one line for each LQ entry (add and remove buttons), check syntax and values
* UI: select mode (mesh, silent, ether) for each interface individually
* UI: manage default-lq for each interface individually
* UI: paramsection for infoplugins (at least for httpinfo subnets/hosts)
* UI: configure "main ip" for routers having multiple public IPs
* establish "links" script in /usr/bin/local, as of this script: https://gist.githubusercontent.com/pocki80/eeea81945111ac14b937bd46b83412d2
* get rid of old code and patches, that are no longer needed.
