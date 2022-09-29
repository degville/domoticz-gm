# domoticz-gm

[![yt-dlp](https://snapcraft.io/domoticz-gm/badge.svg)](https://snapcraft.io/domoticz-gm)

This repository contains Snapcraft build files for [Domoticz](https://github.com/domoticz/domoticz).

Domoticz is a home automation system that lets you monitor and configure various devices like lights, switches, various sensors/meters like temperature, rain, wind, UV, gas, water and much more.

The snap can be manually built by cloning this project and running the _snapcraft_ command in its root.

See [https://snapcraft.io/docs/service-management](https://snapcraft.io/docs/service-management) for help on stopping, enabling and disabling services.

This build also has experimental settings support for HTTP and HTTPS ports, along with loglevel.

You set them as follows (each should trigger a restart):

```bash
sudo snap set domoticz-gm ports.https=444
sudo snap set domoticz-gm ports.http=8090
sudo snap set domoticz-gm loglevel=2
```

Retrieve settings with snap get:

```
$ sudo snap get domoticz-gm ports
Key          Value
ports.http   8090
ports.https  444
```
 
For more details on settings, see: [https://snapcraft.io/docs/configuration-in-snaps](https://snapcraft.io/docs/configuration-in-snaps).

**The snap build is not endorsed by the upstream project but built for my own personal use**
