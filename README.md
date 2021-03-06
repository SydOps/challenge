## Installation on OSX

[ ![Codeship Status for SydOps/challenge](https://codeship.com/projects/78f956d0-7046-0132-f341-227a26fe7ed7/status?branch=master)](https://codeship.com/projects/54503)

Install Vagrant and librarian-puppet

    include Vagrant (http://vagrantup.com) 
    include librarian-puppet (http://librarian-puppet.com/) 
    
Clone the git repository to local disk (need 2GB disk space for each vagrant box)

    git clone https://github.com/SydOps/challenge.git
    
Install all required gems

    bundle install

Install all Puppet modules with Puppet Librarian

    librarian-puppet install

Start all the vms with Vagrant

    vagrant up  (or vagrant up web01 ; vagrant up web02; vagrant up haproxy)

Test the load balancer from your favorite web browser

    http://192.168.50.54
    
Keep refresh, you should see the server name keep changing between web01.example.com and web02.example.com

