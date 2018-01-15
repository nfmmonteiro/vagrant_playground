# Vagrant - Getting Started
This is my first attempt at Vagrant. This project follows the instructions of the [Getting Started Vagrant Tutorial](https://www.vagrantup.com/intro/getting-started/index.html).

## Notes

1. `vagrant init hashicorp/precise64` creates a Vagrantfile with basic Vagrant configuration from a base image hashicorp/precise64 (called box);

2. `vagrant up` boots up the Vagrant environment (starts the Virtual Machine, but without UI)

3. `vagrant ssh` logs into the Virtual Machine

4. `vagrant status` shows the status of the Vagrant boxes

5. teardown:
	1. `vagrant suspend` saves the current state of the box and stop it (fast, but eats up disk space)
	2. `vagrant halt` shutsdown the box (slower than suspend, but eats less disk space)
	3. `vagrant destroy` removes all traces of the box from the host machine

6. `vagrant up` rebuilds the environment. If provision is needed, run `vagrant up --provision` or `vagrant provision`

7. `vagrant plugin install vagrant-vbguest` installs VB Guest Additions plugin.

For more information about Vagrant, go to the [Vagrant Documentation](https://www.vagrantup.com/docs/).
