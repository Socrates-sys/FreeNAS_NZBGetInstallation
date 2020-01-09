# FreeNAS_NZBGetInstallation

1) Install NZBGET in jail
```bash
pkg install nzbget
```

2) In config file `/usr/local/etc/nzbget.conf` set
```bash
WebDir=/usr/local/share/nzbget/webui
ConfigTemplate=/usr/local/share/nzbget/nzbget.conf
ControlUsername=
ControlPassword=
```

3) Enable run on startup
```bash
sysrc 'nzbget_enable=YES'
```

4) Add jail storage for /downloads

5) Restart jail

6) Navigate to {jail-IP}:6789 for NZBGET web interface
