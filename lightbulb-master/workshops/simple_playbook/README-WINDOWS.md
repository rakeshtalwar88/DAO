# Workshop: Simple Playbook

### Topics Covered

* Using `ansible-playbook`
* YAML syntax basics
* Basic Ansible playbook structure
* Tasks and modules

### What You Will Learn

* How to use `ansible-playbook`
* The basics of YAML syntax and Ansible playbook structure

### Before You Begin

If you're not familar with the structure and authoring YAML files take a moment to read thru the Ansible [YAML Syntax](http://docs.ansible.com/ansible/YAMLSyntax.html) guide.

#### NOTE

You will need to assure each host in "web" group has setup the EPEL repository to find and install the nginx package with yum.

### The Assignment

Create an Ansible playbook that targets `client2` host and has the following state:

1. Check that IIS is enabled.
1. Configure a IIS Web site and name it `Ansible: Workshop2` (Hint: check docs `ansible-doc win_iis_website`).
1. Load the homepage that is provided in `resources/` to `C:\inetpub\wwwroot\index.html` (Hint: There is a module in ansible, that copies files to remote locations on windows hosts).

While developing the playbook use the `--syntax-check` to check your work and debug problems. Run your playbook in verbose mode using the `-v` switch to get more information on what Ansible is doing. Try `-vv` and `-vvv` for added verbosity. Also consider running `--check` to do a dry-run as you are developing. 


#### Extra Credit

1. Add a new user on both the hosts by creating an ansible playbook.
1. Run a simple powershell by defining it in the ansible playbook (Hint: `ansible-doc script` ).
1. Run ipconfig command (Hint: Try with raw ansible module)
1. Check if a file exist in the host machine already (Hint: `ansible-doc win_stat`)

### Resources

* [YAML Syntax](http://docs.ansible.com/ansible/YAMLSyntax.html)
* [Intro to Ansible Playbooks](http://docs.ansible.com/ansible/playbooks_intro.html)
* [win_feature module](http://docs.ansible.com/ansible/win_feature_module.html)
* [win_iis_website_module module](http://docs.ansible.com/ansible/win_iis_website_module.html)
* [debug - Print statements during execution](http://docs.ansible.com/ansible/debug_module.html)
* [Windows modules](http://docs.ansible.com/ansible/list_of_windows_modules.html)

