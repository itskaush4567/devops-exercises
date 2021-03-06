# Outcome 11 - Securing Deployments

An exercise that covers the following operations:
  - Setting up hooks to scan for secure credentials/token before code is checked in to a repo
  - Ensuring credentials for production systems are stored in a secure vault and restricting access to it
  - Isolating security credentials/tokens for all different environments
  - Putting together tools to monitor and analyze system logs for suspicious activities
  - Running processes with the least required set of permissions to prevent privilege escalation
  - Setting up and configuring ssh daemon for private key authentication
  - Applying OS security patches to a system
  - Defining firewall rules to control access to the machine
  - Logging all connections to deployed machines
  - Securing data transfer using SSL

### System Requirements
* Python
* Pip
* Ansible > 2.0
* AWS CLI (installed in virtual machine or remote server)
* Boto
* Ruby
* Cucumber
* Virtual box (to test locally)


# Testing locally

### Setup
* Run `vagrant up`. This will bring up a virtual machine and also provision it.
* Update the variables in _vars.yml_ file with yours. Note that _host_user_ should be changed to `vagrant` and not `ubuntu` for testing locally.

### Run tests
* Run cucumber features/git_hook_setup_steps.feature to run tests and set up hooks to scan for secure credentials/token before code is checked in to a repo in the virtual machine.
