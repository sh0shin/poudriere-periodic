# poudriere-periodic

A daily FreeBSD periodic script for poudriere.

## installation

	install -m 0555 540.poudriere /usr/local/etc/periodic/daily/

### periodic.conf example

	## 540.poudriere
	daily_poudriere_update_ports_enable="YES"           # default: YES
	daily_poudriere_update_ports_name="myports"         # default: default

	daily_poudriere_check_bulk_enable="YES"             # default: NO
	daily_poudriere_check_bulk_jails="myjail"           # default: all jails
	daily_poudriere_check_bulk_pkglist="path/to/mypkgs" # default: /usr/local/etc/poudriere.d/ports-list

