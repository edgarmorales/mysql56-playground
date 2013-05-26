# MySQL 5.6 Playground

Fires up a virtual machine with MySQL 5.6 installed, and provides scripts to
backup and restore our app-test database.  All you need to do is:

    vagrant up

During provisioning, you'll notice that MySQL 5.5 gets installed.  Don't panic,
that's just to get some of the system dependencies in place, as the manual
dpkg install of MySQL 5.6 doesn't do all that.

Proisioning the first time may take some time, as the VM first has to download
the mysql deb file, which is 256MB.  The file will be saved into the vagrant repo
root to be reused if you destroy the vm.

Once provisioning is complete, you'll have a virtual machine with MySQL 5.6 up
and running.

    vagrant ssh
    mysql -u root

