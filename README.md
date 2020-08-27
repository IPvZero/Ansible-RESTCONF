# ANSIBLE RESTCONF LAB
Deploying iBGP, EIGRP, SNMP, Syslog and NTP over RESTCONF via Ansible

-----------------------------------------------------------------------------------
# LAB SETUP

To Begin this Lab, first configure construct a topology as follows:
TOPOLOGY:


![alt text](https://github.com/IPvZero/Ansible-RESTCONF/blob/master/images/labpic.png?raw=true)

NOTE: For a quickstart, simple copy-paste the base configurations from the Startupconfig folder in this repo.
Be aware that you will have to change the management IP address to match your own setup - in my case, I'm using the 192.168.31.0/24 network as MGMT.

I have also configured name resolution in my /etc/hosts file. As such, I have no IP addresses explicitly configured in my Ansible inventory.yml file.
Instead I have simply stated the device name - which with then be resolved to the respective MGMT ip addresses. See below:


![alt text](https://github.com/IPvZero/Ansible-RESTCONF/blob/master/images/etc.png?raw=true)

----------------------------------------------------------------------------------------------------
# EXECUTION

Once you have each device configured with their basic startup configs, you can deploy the playbook simply by typing: 


```ansible-playbook restconf-playbook.yml```

-------------------------------------------------------------------------------------------------------------------
# OUTPUT

Your network should now be configured!


![alt text](https://github.com/IPvZero/Ansible-RESTCONF/blob/master/images/complete.png?raw=true)


-----------------------------------------------------------------------------------------------------------------

### Contact Me:

[Twitter](https://twitter.com/IPvZero)

[Youtube](https://youtube.com/c/IPvZero)

