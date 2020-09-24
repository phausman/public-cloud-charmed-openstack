# Public Cloud Charmed OpenStack

This repository contains juju bundles that deploy Charmed OpenStack control
plane in the public cloud (AWS) and nova-compute units in a MAAS-controled
bare-metal machines. Juju cross model relations are used for connecing compute
units with the control plane.

# Control plane architecture

OpenStack charms:

- cinder
- glance
- keystone
- neutron-api
- nova-cloud-controller
- openstack-dashboard
- placement

Supporting charms:

- percona-cluster
- rabbitmq-server

# Compute plane architecture

OpenStack charms: 

- nova-compute
- neutron-gateway
- neutron-openvswitch

Supporting charms:

- ntp

# Deployment procedure

See detailed instruction in the following Google Doc:
https://docs.google.com/document/d/1gJAlWFuZ2p41tkNT3ZdVETwf6DWFqoHoIYawgm9kfCI/