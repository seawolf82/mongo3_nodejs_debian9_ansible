# mongo3_nodejs_debian9

This script install on debian9 mongodb CE version 3.6 and nodejs 10


To install mongo3_nodejs_debian9 on debian 9 run:

ansible-playbook -i hosts site.yaml

To uninstall mongo3_nodejs_debian9 on debian9 run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
mongodb
nodejs


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
