# Workshop: Ad-Hoc Commands for Windows

### Topics Covered

* Ansible Modules
* Facts
* Inventory and Groups
* `ansible` command-line options: ```-i -m -a -b --limit```

### What You Will Learn

* How to test your Ansible configuration and connectivity
* How to get and display Ansible facts
* How to install a package

### The Assignment

Perform the following operations using ad-hoc commands:

1. Test that Ansible is setup correctly to communicate with all hosts in your inventory using the `win_ping` module.
1. Fetch and display to STDOUT Ansible facts using the `setup` module.
1. Install following Windows features (`Web-Server,Web-Common-Http`) using `win_feature` module on `client1` host only.
1. Run the whoami command on all hosts using the `win_shell` module. 

#### Extra Credit

1. Fetch and display only the "virtual" subset of facts for each host.
1. Fetch and display the value of fully qualified domain name (FQDN) of each host from their Ansible facts.
1. Copy a file on remote host (`client1`) from one source to the another using the `win_copy` module (Hint: Set remote_src to True).
1. Ping all hosts **except** the 'client2' host using the `--limit` option

### Reference

* `ansible --help`
* [win_ping module](http://docs.ansible.com/ansible/ping_module.html)
* [setup module](http://docs.ansible.com/ansible/setup_module.html)
* [win_feature module](http://docs.ansible.com/ansible/win_feature_module.html)
* [win_shell module](http://docs.ansible.com/ansible/win_shell_module.html)
* [Introduction To Ad-Hoc Commands](http://docs.ansible.com/ansible/intro_adhoc.html)
* [Windows modules](http://docs.ansible.com/ansible/list_of_windows_modules.html)
