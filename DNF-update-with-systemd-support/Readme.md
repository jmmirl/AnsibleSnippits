
DNF Update with SystemD integration 

 

Install the script on the destination host. 

ansible-playbook -i 172.24.17.174, --user=ec2-user inventory setup_patch_host.yml --key-file "my-keypair.pem"

Enable the systemd timers and logrotate management. 

ansible-playbook -i 172.24.17.174, --user=ec2-user inventory configure_patch_system.yml --key-file "my-keypair.pem"
