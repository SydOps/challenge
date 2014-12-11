Build a set of scripts to provision and maintain a configurable number of virtual servers.
 
The solution should include:
  * A front end load balancer (that will route HTTP requests to multiple app servers)
  * 1 or more app servers (that will return a HTML response showing the current IP address of the server)
  * The ability to easily update the scripts to add and remove app servers from the cluster
 
The scripts should be able to run on OSX and can utilise any tools (such as Vagrant/Docker and Chef/Puppet/Ansible).
