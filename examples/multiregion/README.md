Multi regions Openstack Network
==========

Configuration in this directory creates set of openstack resources which bootstraps a multi region network
using the OVH Vrack.

There are 3 private subnets created in addition to 3 NAT Gateway in 3 regions.

Usage
=====

To run this example you need to execute:

```bash
$ terraform init
$ terraform apply -var project_id=... -var vrack_id=...
```

Note that this example may create resources which can cost money (Openstack Instance, for example). Run `terraform destroy` when you don't need these resources.
