#This ansible runbook was created to install the zabbix agents in Linux
#I have 2 yml files to use for installation of the agents in stage and prod environments (The std we follow in our company)
#This cookbook installs the zabbix agent version 2.2.2, but can be modified to install any agent version (Tweaks required in tasks/zabbix_install_v2_2_2.yml)
#The related rpms must be placed in rpms folder
#The hosts in which this should be installed should be added to "hosts" file
#The ansible playbook command that I use is below,
	#ansible-playbook -v -i /path/tothe/folder/hosts -k -K zabbixhostsprod.yml --extra-vars "user=<username>"
	#ansible-playbook -v -i /path/tothe/folder/hosts -k -K zabbixhostsstage.yml --extra-vars "user=<username>"
#Use either one of the yml file depending on if you are going to install the agent in stage or prod.
#You can also create a single yml file if you do not require the stage/prod distinction	
