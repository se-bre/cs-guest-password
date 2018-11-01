## Ubuntu 18.04

**tested:** Ubuntu 18.04

- reset root password  
- fix missing ssh host keys  
- hostname handling

.service file to `/etc/systemd/system/cloudstack-init.service`  

	systemctl daemon-reload

enable service

	systemctl enable cloudstack-init.service

`/usr/bin/cloudstack-init`

	chmod +x /usr/bin/cloudstack-init

---
**hint** at the moment only working for IPv4
