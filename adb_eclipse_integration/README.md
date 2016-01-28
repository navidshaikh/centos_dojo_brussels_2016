# [vagrant-adbinfo](https://github.com/projectatomic/vagrant-adbinfo) Vagrant Plugin

Provide setup information, including environment variables and certificates, required to access services provided by an [Atomic Developer Bundle (ADB)](https://github.com/projectatomic/adb-atomic-developer-bundle).  This plugin makes it easier to use the ADB with host-based tools such as Eclipse and the docker and kubernetes CLI commands.  Details on this usage pattern can be found in the [ADB Documentation](https://github.com/projectatomic/adb-atomic-developer-bundle/blob/master/docs/using.rst).

The [Atomic Developer Bundle](https://github.com/projectatomic/adb-atomic-developer-bundle) is  Vagrant box that provides a ready-to-use development environment for container applications. With ADB, developers can dive right into producing complex, multi-container applications.

## Quick Start

1. Install and start the Atomic Developer Bundle (ADB), as [documented](https://github.com/projectatomic/adb-atomic-developer-bundle/blob/master/docs/installing.rst) in the ADB project.

2. Install the vagrant-adbinfo plugin

        vagrant plugin install vagrant-adbinfo

3. Run the plugin to get environment variables and certificates

        $ vagrant adbinfo
        Set the following environment variables to enable access to the
        docker daemon running inside of the vagrant virtual machine:

        export DOCKER_HOST=tcp://172.13.14.1:2376
        export DOCKER_CERT_PATH=/home/bexelbie/Repositories/vagrant-adbinfo/.vagrant/machines/default/virtualbox/.docker
        export DOCKER_TLS_VERIFY=1
        export DOCKER_MACHINE_NAME="90d3e96"

4. Begin using your host-based tools.

## Get Involved/Contact Us

  * IRC: #atomic and #nulecule on freenode
  * Mailing List: container-tools@redhat.com
