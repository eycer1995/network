# This is my homelab

[diagram](network/src/diagram.png)

My homelab is a playground that I use to test different technologies and study
without worrying too much about making mistakes, because that's the best way to
learn, trial and error.

This diagram was made using [draw.io](draw.io)

#### Currently working on:
* Improve my containerization knowledge
* Migrating everything from docker to podman
* Improve ansible skills

## Setup
---
###### Raspberry Pi 4B+
Hardware specs:
* Processor: ARM Cortex-A72 @ 1.50GHz
* RAM: 4GiB
* Disk 0: 120G SandDisk MicroSD
* Disk 1: Seagate 4TB HDD USB 3.0
* Network: 1Gbit/s
* OS: Raspbian Lite 64 bit

Network configuration:
* IP address: 192.168.0.101
* Hostname: rpi01

Services running (podman containers):
* Jellyfin
* Transmission
* Sonarr
* Jackett

##### Raspberry Pi 3B+
Hardware specs:
* Processor: ARM Cortex-A53 @ 1.40GHz
* RAM: 1GiB
* Disk 0: 32G SandDisk MicroSD
* Network: eth0 not used, wlan0 IEEE 802.11 (11Mbit/s)
* OS: Raspbian Lite 64 bit

Network configuration:
* IP address: 192.168.0.102
* Hostname: rpi02

Services running (bare metal):
* Pihole
* Pivpn Wireguard

##### Packard Bell
Hardware specs:
* Processor: Pentium(R) Dual-Core CPU T4300  @ 2.10GHz
* RAM: 4GiB (2x2GiB) DDR2
* Disk 0: 640GB HDD
* Network: 100Mbit/s
* OS: Debian 11 64 bit

Network configuration:
* IP address: 192.168.0.126
* Hostname: bell

Services running (docker containers):
* Nginx Proxy Manager + mariadb
* Up-time Kuma
* Grafana + InfluxDB + Telegraf
* Bookstack
* Calibre-web
* Nextcloud
* Portainer

##### Desktop Fedora
Hardware specs:
* Processor: Intel(R) Core(TM) i3-8100 CPU @ 3.60GHz
* RAM: 12GiB DDR4 2400MHz
* Disk 0: ATA Disk KINGSTON SA400S3 480GB SSD
* Disk 1 (odin): ATA Disk ST1000DM010-2EP1 1TB HDD
* Network: 1Gbit/s
* OS: Fedora 35

Services running (Virutalbox):
* Minecraft server
* Centos vm for testing
* Debian vm for testing
