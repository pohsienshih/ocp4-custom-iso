Playbook to create custom ISO files for each OCP node.

1. Edit inventory file 
- all hosts' IP, FQDN etc
- network interface name, netmask, gateway, dns server, install device, http server
- check that the metal bios and RHCOS ISO file names (version) and file paths match

2. Add RHCOS ISO file to `roles/custom_iso/files/`

2. Run playbook
`ansible-playbook custom-iso.yml`
- to run as root: `ansible-playbook custom-iso.yml --ask-become-pass` 
