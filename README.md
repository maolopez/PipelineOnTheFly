PipelineOn The Fly
==================

You have to finish the Jenkins server configuration manually: Install plugins.


|*CloudFormation template*                  |*Description*                                 |*Usage*             |
| ------------------------------------------|:--------------------------------------------:|:-------------------|
|ansible-jenkins-infra.yaml                 |Jenkis/Public, Ansible/Private, server/subnet |AWS CloudFormation  |
|saltnjenkinsinfra.yaml                     |Jenkis/Public, Salt/Private, servers/subnet   |AWS CloudFormation  | 
|infra-4-ut-anagramma.yaml                  |Jenkis/Public + 2 instances/Public            |AWS CloudFormation  |



Steps for the infrastructure with Salt Master and Minion
--------------------------------------------------------

1. The Jenkins server works as a bastion host. Copy your SSH pair keys in order to access the 
   instances in the private subnet.
2. Go to the minion /etc/hosts file and include the Salt Master's IP salt.
3. Restart salt-minion service
4. You will recognize the Sal Master because /etc/hosts -> 127.0.0.1 salt.
5. In the salt-master accept the keys

Steps for the infrastructure with Ansible server
------------------------------------------------

1. The Jenkins server works as a bastion host. Copy your SSH pair keys in order to access the 
   instances in the private subnet. 

Steps for the infrastructure for Ut-Anagramma demo
--------------------------------------------------

1. The Jenkins server and a server for Dev and a server for Prod.

see: https://github.com/maolopez/ut_anagramma

