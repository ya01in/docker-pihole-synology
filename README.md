# docker-pihole-synology

A Pi-hole Docker Compose for deploying on Synology NAS

## Description

Pi-hole is a [DNS sinkhole](https://en.wikipedia.org/wiki/DNS_sinkhole) is to create a personal domain name sinkhole to block you from accidentally accessing unwanted domains like advertisements and trackers while browsing the web. Saving your bandwidth for what you intended.
It is built with rich features such as DNS client/group management, and a DHCP server if needed.
Originally designed for Raspberry Pi, but you can set up one using Docker.

This is a Docker Compose for [Pi-hole](https://hub.docker.com/r/pihole/pihole) on Synology NAS.
I currently can access the admin page through reverse proxy, and clients connected through the VPN Server also can use it.

## Environment setup

### NAS

- Model: DS923+
- DSM VERSION: DSM 7.2.2-72806 Update 3
- Container Manager (Docker) Version: 24.0.2-1535

### Pi-hole

- TAG: latest
- SHA256: `feb8c881adba50db1a084d9818946051d6c439d04910b6bcecb7a644449e9fa8`

## Note

### The Pi-hole instance IPv4 is wrong

After testing with different settings in Docker Compose. **Without modifying DSM or Docker,** I think it is caused by DSM not wanting people to directly access the system's network.
A bit annoying but won't cause any problems.

Happy Tinkering~ Wish you a quiet web
