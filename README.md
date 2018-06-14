# ER-wizard-OLSRd_V1
OLSRd (V1) Wizard for Ubiquiti EdgeMAX Devices supporting Wizards

branch to prepare new release including 0.9.7

what to work on:
* new olsrd packages
* fix paths to plugins (dynamically?)
* tune default parameters of info-plugins (especialle httpinfo plugin allowed hosts/subnets)
* new etc-init.d scripts including logging and watchdog handling
* new config sections, one for each activated interface
* remove interfaces from startup-parameters
* HNAs into default interface section
* UI: one hna entry and subnet for each line (add and remove buttons)
* UI: select mode (mesh, silent, ether) for each interface individually
* UI: configure "main ip"
* UI: paramsection for infoplugins (at least for httpinfo subnets/hosts)
* activate httpinfo, watchdog on install "by default"?
* establish "links" script in /usr/bin/local, as of this script: https://gist.githubusercontent.com/pocki80/eeea81945111ac14b937bd46b83412d2
