# Tomcat deployment with Ansible

This project contains an ansible playbook which downloads a given version of
Tomcat from the Maven Central repository and install it in the `tomcat`
repository of the current directory on the managed target machine.

The aim of the project is not to provide a production ready instance of Tomcat,
but a way to test ansible on a local machine.  

# Prerequisite

Ansible is supposed to be installed on the machine you execute this example.
We also provide a Vagrant over Virtual Box VM setup. The project contains
an inventory which uses the Vagrant VM with the ip address `192.168.33.10`.

# Execution

Set the VM up with
```shell script
$ vagrant up
```

Destroy (clean) the VM with
```shell script
$ vagrant destroy
```

Run the ansible playbook using the following script:
```shell script
$ ./run-playbook.sh
```
