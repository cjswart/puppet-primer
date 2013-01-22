puppet-primer
=============

Prerequisites
-------------
Have the following software installed:
* VirtualBox 4.2.x - https://www.virtualbox.org/wiki/Downloads
* Vagrant 1.0.6 - http://downloads.vagrantup.com

Initialization
--------------
Download and add a CentOS 6.3 box for vagrant:
    vagrant box add centos63 https://dl.dropbox.com/u/7225008/Vagrant/CentOS-6.3-x86_64-minimal.box

Start the image:
    vagrant up

The following output will be shown when puppet runs successfully:
    [default] Running Puppet with /tmp/vagrant-puppet/manifests/primer.pp...
    notice: Hello
    
    notice: /Stage[main]//Notify[Hello]/message: defined 'message' as 'Hello'
    
    notice: Finished catalog run in 0.03 seconds

Run puppet (again):
    vagrant provision

