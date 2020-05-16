Playbook to create custom ISO files for each OCP node.

1. Edit inventory file 
Include all hosts' IP, FQDN etc

2. Add RHCOS ISO file to `roles/custom_iso/files/`

2. Run playbook
`ansible-playbook custom-iso.yml`
