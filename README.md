Introduction
============

This is a Docker container to run [smokeping](https://oss.oetiker.ch/smokeping/),
based on CentOS 7.

Configuration
=============

By default, this container uses the default example configuration file provided
with smokeping. If you wish to customize the configuration, you should bind
mount your custom configuration file onto `/etc/smokeping/config`.

Persistent Data
===============

The persistent data for this container all lives within `/var/lib/smokeping/rrd`.
If you want this data to persist over container restarts, please bind mount a
directory from your host into this container.
