# MAAS (Metal as a Service) Charms

Juju charms that allow deploying both the MAAS region controller and MAAS rack
controller.

The MAAS region controller is the main communication point for MAAS. Users and
tools communicate over the API and UI frontend to control machines and devices.
The following services are installed and setup with the maas-region charm:

* bind9
* haproxy
* keepalived (only with vip config is set)
* maas-proxy
* maas-regiond

The MAAS rack controller is where BMC's for machines are controller where the
machines PXE boot, download images, and contact for DHCP. The following
services are installed and setup with the maas-rack charm:

* maas-dhcpd
* maas-dhcpd6
* maas-rackd
* tgtd

For more information see [MAAS]((https://maas.io)).

## Scale out Usage

*TODO*

## Known Limitations and Issues

*Not production ready*

# Configuration

*TODO*