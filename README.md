PipelineOn The Fly
==================

You have to finish the Jenkins server configuration manually.


Usage
-----

In Construction 


Steps for the pipeline with Salt Master and Minion
----------------------------------------------------

1. The Jenkins server works as a bastion host. Copy your SSH pair keys in order to access the 
   instances in the private subnet.
2. Go to the minion /etc/hosts file and include the Salt Master's IP salt.
3. Restart salt-minion service
4. You will recognize the Sal Master because /etc/hosts -> 127.0.0.1 salt.
5. In the salt-master accept the keys

Steps
----------------------------------------------------

1. 
