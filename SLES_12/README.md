## SLES 12

**tested:** SLES 12 SP3

.service file to `/etc/systemd/system/cloud-set-guest-password.service`  

	systemctl daemon-reload

enable service

	systemctl enable cloud-set-guest-password.service

`/usr/bin/cloud-set-guest-password`

	chmod +x /usr/bin/cloud-set-guest-password

---
**hint** at the moment only working for IPv4

