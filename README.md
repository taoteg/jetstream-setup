# jetstream-setup

This repository contains simple examples to quickly set up a standard Jetstream image with Docker, Globus Personal Connect, Singularity, and other useful tools.

Also included are some large-ish Docker images that we pull at setup time so they are ready to go, but because they are on the large-ish side you probably want to use at least an [m1.small Jetstream instance (2 vCPUs, 4GB RAM, 20 GB local storage, 2 SUs/hour)](http://jetstream-cloud.org/general-vms.php).

Assumes that you are using the Ubuntu image curated by the Jetstream admins, specifically: [Ubuntu 14.04.3 Development GUI](https://use.jetstream-cloud.org/application/images/54)

Currently installs as of 2017-03-24:

```bash
DOCKER_VERSION=17.03.0~ce-0
GLOBUS_VERSION=2.3.3
SINGULARITY_VERSION=2.2.1
```

Read the [official instructions](https://docs.docker.com/engine/installation/linux/ubuntu/) to install the latest version of Docker.

## Quickstart
On a freshly-created Jetstream instance, become root and then download and run the setup script using these commands:

```bash
$ sudo -i
# bash -ex <(curl -s https://raw.githubusercontent.com/aculich/jetstream-setup/master/jetstream-setup.sh)
```
