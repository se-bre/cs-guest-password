## Ubuntu 18.04

**tested:** Ubuntu 18.04

[features](#features)  
[create/enable service](#service)  
[create script](#script)  
[logfiles](#logfiles)  
[hints](#hints)  

---

#### features

- reset root password  
- fix missing ssh host keys  
- hostname handling

---

#### service  

.service file to `/etc/systemd/system/cloudstack-init.service`  

	systemctl daemon-reload

enable service

	systemctl enable cloudstack-init.service

---

#### script  

move cloudstack-init to `/usr/bin/cloudstack-init` and adjust permissions

	chmod +x /usr/bin/cloudstack-init

---

#### logfiles

show service logs

	journalctl -u cloudstack-init.service

---

#### hints  

- at the moment only tested with IPv4
- on hostname change complete `/etc/hosts` will be rewritten
