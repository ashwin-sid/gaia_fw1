Role Name
=========

Using this role you can easily automate essential tasks for your Checkpoint Gaia Firewalls. You can do the following by using this role: -
•	Take clish config back-ups ( show configuration )
•	Run essential show commands on all your gateways from single playbook.eg. 
        o	Show route 
        o	Show asset all 
        o	Show interfaces 
        o	Show ospf , etc… 
•	Issue configure commands to all your gateways from single playbook. 

Requirements
------------

The requirements are as follows:- 
•	Linux server. The role has been tested with RHEL 7+ and Ubuntu, but it should work with other flavours as well. 
•	Ansible 2.5 and above running on the Linux server. 
•	Direct connection to the checkpoint firewalls (at the moment the role does not support jump box) . 

Role Variables
--------------

The Role has the following defaults:- (but all of these can be changed) 
•	Username to login to the firewall is 'admin', this can be changed per firewall in the inventory file.
•	ssh port is 22, again if you are using a custom port this can be changed in the inventory file. 


Example Playbook
----------------

Sample Playbooks are included in folder 'Sample-playbook'. Please visit my blog for further examples and more detailed implementation: - 
Please Visit - "http://ash-sidhu.blog/2018/11/07/using-ansible-for-automating-tasks-on-checkpoin t-firewall" 
for more detailed implementation procedure.

UPDATE NOTE (25/02/19) : I have added provision to add custom output directory. Variable 'logdir', you can specify where the output gets stored. The Sample-playbooks reflect this.  


License
-------

GPLv3

Author Information
------------------

Please visit my blog for further examples and more detailed implementation: - 

"http://ash-sidhu.blog/2018/11/07/using-ansible-for-automating-tasks-on-checkpoin t-firewall"
