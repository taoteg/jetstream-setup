# jetstream-setup

This repository contains simple examples to quickly set up a standard Jetstream image with Docker, Globus Personal Connect, Singularity, and other useful tools.

Also included are some large-ish Docker images that we pull at setup time so they are ready to go, but because they are on the large-ish side you probably want to use at least an [m1.small Jetstream instance (2 vCPUs, 4GB RAM, 20 GB local storage, 2 SUs/hour)](http://jetstream-cloud.org/general-vms.php).

Assumes that you are using the Ubuntu image curated by the Jetstream admins, specifically: [Ubuntu 14.04.3 Development GUI](https://use.jetstream-cloud.org/application/images/54)

Currently installs:

- latest version (non-pinned) of Docker from the [official instructions](https://docs.docker.com/engine/installation/linux/ubuntu/)

