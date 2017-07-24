## IPSec Networking

Rancher networking plugin using IPsec.

### Open Ports

Traffic to and from hosts require UDP ports `500` and `4500` to be open.

### Changelog - 0.1.2

This version removes the `cni-driver` service as a sidekick of the `ipsec` service and makes it standalone.

#### [rancher/net:v0.11.4]
* Fixed an issue where custom subnets were forcing `/16`

### Usage

#### Configuration options
* `RANCHER_DEBUG`

##### [cni-driver]

* `DOCKER_BRIDGE`
* `MTU`
* `SUBNET`
* `RANCHER_HAIRPIN_MODE`
* `RANCHER_PROMISCUOUS_MODE`
* `HOST_PORTS`
* `SUBNET_PREFIX`
