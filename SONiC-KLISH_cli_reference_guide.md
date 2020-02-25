# The SONiC CLI Reference Guide 

Contents
========
!https://raw.githubusercontent.com

## aaa authentication failthrough 

#### Description 

AAA authentication failthrough status 

#### Parent Commands (Modes) 

`config t`

#### Syntax 

```
aaa authentication failthrough <enable>
```
#### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| enable | enable or disable  | Select [enable(enable) disable(disable) ]  |


## aaa authentication login-method 
#### Description 

AAA authentication login method preference 

#### Parent Commands (Modes) 
`config t`

#### Syntax 
```
aaa authentication login-method { { [ local ] [ <tacacs+> ] [ <radius> ] } | { [ tacacs+ ] [ <local> ] } | { [ radius ] [ <local> ] } }
no aaa authentication login-method
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tacacs+ |   | Select [tacacs+(tacacs+) ]  |
| radius |   | Select [radius(radius) ]  |
| local |   | Select [local(local) ]  |
## activate 
#### Description 

This command enables/activates a particular address-family for a BGP
neighbor

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
activate
no activate
```
#### Usage Guidelines 

Use this command to activate an address-family for a BGP neighbor.
This command can be executed multiple times to enable multiple address
familities for a BGP neighbor

#### Examples 
Following command enables ipv4 unicast address family            for a BGP neighbor 20.20.20.2 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# activate
```
## activate 
#### Description 

This command enables/activates a particular address-family for a BGP
peer-group

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
activate
no activate
```
#### Usage Guidelines 

Use this command to activate an address-family for a BGP peer-group.
This command can be executed multiple times to enable multiple address
familities for a BGP peer-group

#### Examples 
Following command enables ipv4 unicast address family            for a BGP peer-group PG_External 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# remote-as 300
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# activate
```
## activate 
#### Description 

Enable the Address Family for this Neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
activate
no activate
```
## activate 
#### Description 

Enable the Address Family for this Neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
activate
no activate
```
## activate 
#### Description 

Enable the Address Family for this Neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
activate
no activate
```
## activate 
#### Description 

Enable the Address Family for this Neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
activate
no activate
```
## addpath-tx-all-paths 
#### Description 

This command enables BGP to advertise all paths to a neighbor.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
#### Usage Guidelines 

Use this command for BGP add path feature configuration. This command
allows all BGP paths to be advertised to a neighbor

#### Examples 
Following command configures BGP to advertise          all paths to a neighbor 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# addpath-tx-all-paths
```
## addpath-tx-all-paths 
#### Description 

This command enables BGP to advertise all paths to neighbors in a
peer-group.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
#### Usage Guidelines 

Use this command for BGP add path feature configuration. This command
allows all BGP paths to be advertised to neighbors in a peer-group

#### Examples 
Following command configures BGP to advertise all paths           to neighbors in a peer-group 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# addpath-tx-all-paths
```
## addpath-tx-all-paths 
#### Description 

Use addpath to advertise all paths to a neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
## addpath-tx-all-paths 
#### Description 

Use addpath to advertise all paths to a neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
## addpath-tx-all-paths 
#### Description 

Use addpath to advertise all paths to a neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
## addpath-tx-all-paths 
#### Description 

Use addpath to advertise all paths to a neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
addpath-tx-all-paths
no addpath-tx-all-paths
```
## addpath-tx-bestpath-per-AS 
#### Description 
This command enables BGP to advertise best paths to a neighbor.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
#### Usage Guidelines 

Use this command for BGP add path feature configuration. This command
allows best BGP path to be advertised to a neighbor

#### Examples 
Following command configures BGP to advertise best path to a neighbor 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# addpath-tx-bestpath-per-AS
```
## addpath-tx-bestpath-per-AS 
#### Description 

This command enables BGP to advertise best paths to neighbors in a
peer-group.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
#### Usage Guidelines 

Use this command for BGP add path feature configuration. This command
allows best BGP path to be advertised to neighbors in a peer-group

#### Examples 
Following command configures BGP to advertise best path          to neighbors in a peer-group 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# addpath-tx-bestpath-per-AS
```
## addpath-tx-bestpath-per-AS 
#### Description 

Use addpath to advertise the bestpath per each neighboring AS 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
## addpath-tx-bestpath-per-AS 
#### Description 

Use addpath to advertise the bestpath per each neighboring AS 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
## addpath-tx-bestpath-per-AS 
#### Description 

Use addpath to advertise the bestpath per each neighboring AS 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
## addpath-tx-bestpath-per-AS 
#### Description 

Use addpath to advertise the bestpath per each neighboring AS 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
addpath-tx-bestpath-per-AS
no addpath-tx-bestpath-per-AS
```
## address-family ipv4 
#### Description 

This command enters into IPv4 Unicast address-family configure CLI
context

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
address-family ipv4 unicast
no address-family ipv4 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv4 Unicast address family CLI context to
configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv4 Unicast          address family 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)#
```
## address-family ipv4 
#### Description 

This command enters into IPv4 Unicast address-family configuration CLI
context for a BGP neighbor

#### Parent Commands (Modes) 

`neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }`

#### Syntax 
```
address-family ipv4 unicast
no address-family ipv4 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv4 Unicast address family CLI context of
a BGP neighbor to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv4 Unicast          address family for neighbor 30.30.30.3 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)#
```
## address-family ipv4 
#### Description 

This command switches the CLI context into IPv4 Unicast address-family
mode for a BGP peer-group

#### Parent Commands (Modes) 

`peer-group <template-str>`

#### Syntax 
```
address-family ipv4 unicast
no address-family ipv4 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv4 Unicast address family CLI context of
a BGP peer-group to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv4 Unicast          address family for peer-group PG_Ext 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)#
```
## address-family ipv6 
#### Description 

This command execution enters into IPv6 Unicast address-family configure CLI
context

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
address-family ipv6 unicast
no address-family ipv6 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv6 Unicast address family CLI context to
configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv6 Unicast          address family 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# address-family ipv6 unicast
sonic(config-router-bgp-af)#
```
## address-family ipv6 
#### Description 

This command execution enters into IPv6 Unicast address-family configuration CLI
context for a BGP neighbor

#### Parent Commands (Modes) 

`neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }`

#### Syntax 
```
address-family ipv6 unicast
no address-family ipv6 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv6 Unicast address family CLI context of
a BGP neighbor to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv6 Unicast          address family for neighbor 30.30.30.3 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# address-family ipv6 unicast
sonic(config-router-bgp-neighbor-af)#
```
## address-family ipv6 
#### Description 

This command switches the CLI context into IPv6 Unicast address-family
mode for a BGP peer-group

#### Parent Commands (Modes) 

`peer-group <template-str>`

#### Syntax 
```
address-family ipv6 unicast
no address-family ipv6 unicast
```
#### Usage Guidelines 

Use this command to switch to IPv6 Unicast address family CLI context of
a BGP peer-group to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to IPv6 Unicast          address family for peer-group PG_Ext 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv6 unicast
sonic(config-router-bgp-pg-af)#
```
## address-family l2vpn 
#### Description 

This command execution enters into l2vpn evpn address-family configure CLI
context

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
address-family l2vpn evpn
no address-family l2vpn evpn
```
#### Usage Guidelines 

Use this command to switch to l2vpn evpn address family CLI context to
configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to l2vpn evpn          address family 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# address-family l2vpn evpn
sonic(config-router-bgp-af)#
```
## address-family l2vpn 
#### Description 

This command execution enters into L2VPN EVPN address-family configuration CLI
context for a BGP neighbor

#### Parent Commands (Modes) 

`neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }`

#### Syntax 
```
address-family l2vpn evpn
no address-family l2vpn evpn
```
#### Usage Guidelines 

Use this command to switch to L2VPN EVPN address family CLI context of
a BGP neighbor to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to L2VPN EVPN          address family for neighbor 30.30.30.3 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# address-family l2vpn evpn
sonic(config-router-bgp-neighbor-af)#
```
## address-family l2vpn 
#### Description 

This command switches the CLI context into L2VPN EVPN address-family
mode for a BGP peer-group

#### Parent Commands (Modes) 
```
peer-group <template-str>
```
#### Syntax 
```
address-family l2vpn evpn
no address-family l2vpn evpn
```
#### Usage Guidelines 

Use this command to switch to L2VPN EVPN address family CLI context of
a BGP peer-group to configure parameters specific to this address family

#### Examples 
Below command switches the CLI context to L2VPN EVPN          address family for peer-group PG_Ext 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family l2vpn evpn
sonic(config-router-bgp-pg-af)#
```
## advertise ipv4 unicast 
#### Description 
SAFI unicast 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
advertise ipv4 unicast
no advertise ipv4 unicast
```
## advertise ipv6 unicast 
#### Description 

SAFI unicast 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
advertise ipv6 unicast
no advertise ipv6 unicast
```
## advertise-all-vni 
#### Description 

Advertise all local VNIs 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
advertise-all-vni
no advertise-all-vni
```
## advertise-default-gw 
#### Description 

Advertise all default gw mac-ip routes in EVPN 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
advertise-default-gw
no advertise-default-gw
```
## advertise-default-gw 
#### Description 

Advertise all default gw mac-ip routes in EVPN 

#### Parent Commands (Modes) 

`vni <vninum>`

#### Syntax 
```
advertise-default-gw
no advertise-default-gw
```
## advertisement-interval 
#### Description 

This command sets the minimum interval between sending BGP routing
updates to a neighbor

#### Parent Commands (Modes) 

`neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }`

#### Syntax 
```
advertisement-interval <tval>
no advertisement-interval
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tval |   | Integer  |

#### Usage Guidelines 

Use this command to set the minmum advertisement interval for BGP
updates

#### Examples 
Following command sets the minimum advertisement          interval to 10sec 

```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# advertisement-interval 10
```
## advertisement-interval 
#### Description 

This command sets the minimum interval between sending BGP routing
updates to neighbors in a peer-group

#### Parent Commands (Modes) 

`peer-group <template-str>`

#### Syntax 
```
advertisement-interval <tval>
no advertisement-interval
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tval |   | Integer  |

#### Usage Guidelines 

Use this command to set the minmum advertisement interval for BGP
updates

#### Examples 
Following command sets the minimum advertisement          interval to 10sec 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# advertisement-interval 10
```
## aggregate-address 
#### Description 

This command configures an aggregate address and enables aggregation of
routes that falls in the aggregate address subnet

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
aggregate-address <prefix> { [ as-set ] [ summary-only ] { [ route-map ] <rtemap> } }
no aggregate-address <prefix> { [ as-set ] [ summary-only ] { [ route-map ] <rtemap> } }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix | A.B.C.D/mask  | String  |
| rtemap | String  | String  |

#### Usage Guidelines 

This command enables user to turn on aggregation of BGP routes.
"summary-only" option filters out all the aggregates routes and only the
aggregate address will be advertised by BGP. "as-set" option will make
sure that AS Path of individual aggregated routes are also included in
the resulting aggregate route. "route-map" option gives user a finer
control over the route's attributes

#### Examples 
This configuration example setup the aggregate-address          under ipv4 address-family 

```
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# aggregate-address 17.35.0.0/16
```
## aggregate-address 
#### Description 

Configure BGP aggregate entries 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
aggregate-address <prefix> { [ as-set ] [ summary-only ] { [ route-map ] <rtemap> } }
no aggregate-address <prefix> { { [ <as-set> ] [ <summary-only> ] } { [ route-map ] <rtemap> } }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix | A::B/mask  | String  |
| rtemap | String  | String  |

## aging-interval 
#### Description 

This command is used to configure an aging-interval for drop-monitor flows configured in the system.The aging interval determines how long the system waits before it decides that drops have ceased on a flow.

#### Parent Commands (Modes) 

`drop-monitor`

#### Syntax 
```
aging-interval <aging-interval-time>
no aging-interval
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| aging-interval-time | Aging interval  | Integer  |

#### Usage Guidelines 

This command is used to configure an aging-interval for drop-monitor flows configured in the system.

#### Example 
##### Configure aging interval 
```
sonic(config-drop-monitor)# aging-interval 6
```
## allowas-in 
#### Description 

This command allows BGP neighbor to accept as-path with it's own AS number
present in it.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

#### Usage Guidelines 

Accepting own AS in an as-path usually results in AS loop. But
sometimes, users add AS number to influence the BGP route selection
process. This command enables user to control when a route with as-path
containing own AS number should be accepted or not. The command also
provides flexibility in terms of maximum number of occurrences of AS
number in as-apth.

#### Examples 
Following command enable BGP neighbor to accept as-path          with it's owne AS number repeated 5 or less number of times 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# allowas-in 5
```
## allowas-in 
#### Description 

This command allows neighbors in a BGP peer-group to accept as-path
with it's own AS number present in it.

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

#### Usage Guidelines 

Accepting own AS in an as-path usually results in AS loop. But
sometimes, users add AS number to influence the BGP route selection
process. This command enables user to control when a route with as-path
containing own AS number should be accepted or not. The command also
provides flexibility in terms of maximum number of occurrences of AS
number in as-apth.

#### Examples 
Following command configured allowas-in for a BGP peer-group PG_External 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# remote-as 300
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# allowas-in
```
## allowas-in 
#### Description 

Allow local AS number in as-path 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

## allowas-in 
#### Description 

Allow local AS number in as-path 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

## allowas-in 
#### Description 

Allow local AS number in as-path 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

## allowas-in 
#### Description 

Allow local AS number in as-path 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
allowas-in { [ <value> ] | [ origin ] }
no allowas-in { [ <value> ] | [ origin ] }
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |

## always-compare-med 
#### Description 

Always compare the MED on routes, even when they were received from
different neighbouring ASes. Setting this option makes the order of
preference of routes more defined, and should eliminate MED induced
oscillations.

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
always-compare-med
no always-compare-med
```
#### Usage Guidelines 

Use this command to instruct BGP to always compare MED values for routes
even if they are from different ASes

#### Examples 
Below command enables always-compare-med parameter 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# always-compare-med
```
## as-override 
#### Description 

This command instructs BGP to override AS Numbers in outbound updates if
aspath equals remote-as

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
as-override
no as-override
```
#### Usage Guidelines 

Use this command to override the as number in outbound updates

#### Examples 
Following command configures BGP to override AS number          in as-path 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# as-override
```
## as-override 
#### Description 

This command instructs BGP to override AS Numbers in outbound updates if
aspath equals remote-as

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

##### Syntax 
```
as-override
no as-override
```
##### Usage Guidelines 

Use this command to override the as number in outbound updates

#### Examples 
Following command configures BGP to override AS number          in as-path 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# as-override
```
## as-override 
#### Description 

Override ASNs in outbound updates if aspath equals remote-as 

#### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
#### Syntax 
```
as-override
no as-override
```
## as-override 
#### Description 

Override ASNs in outbound updates if aspath equals remote-as 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
as-override
no as-override
```
## as-override 
#### Description 

Override ASNs in outbound updates if aspath equals remote-as 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
as-override
no as-override
```
## as-override 
#### Description 

Override ASNs in outbound updates if aspath equals remote-as 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
as-override
no as-override
```
## attribute-unchanged 
#### Description 

This command instructs BGP to propagate route attributes (as-path,
next-hop, med) unchanged to this neighbor

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
#### Usage Guidelines 

Use this command to propagate BGP route attributes unchanged to this
neighbor. User can control which attributes (as-path, next-hop, med) i
will be propagated unchanged.

#### Examples 
Following command configures BGP to propagate next-hop          and as-path unchanged to neighbor 20.20.20.2 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# attribute-unchanged as-path next-hop
```
## attribute-unchanged 
#### Description 

This command instructs BGP to propagate route attributes (as-path,
next-hop, med) unchanged to neighbors in a peer-group

#### Parent Commands (Modes) 

`address-family ipv4 unicast`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
#### Usage Guidelines 

Use this command to propagate BGP route attributes unchanged to
neighbors in a peer-group. User can control which attributes (as-path,
next-hop, med) will be propagated unchanged.

#### Examples 
Following command configures BGP to propagate next-hop           and as-path unchanged to neighbors in a peer-group 
```
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# attribute-unchanged as-path next-hop
```
## attribute-unchanged 
#### Description 

BGP attribute is propagated unchanged to this neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
## attribute-unchanged 
#### Description 

BGP attribute is propagated unchanged to this neighbor 

#### Parent Commands (Modes) 

`address-family ipv6 unicast`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
## attribute-unchanged 
#### Description 

BGP attribute is propagated unchanged to this neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
## attribute-unchanged 
#### Description 

BGP attribute is propagated unchanged to this neighbor 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
attribute-unchanged [ as-path ] [ med ] [ next-hop ]
no attribute-unchanged
```
## autoneg 
#### Description 

Configure autoneg 

#### Parent Commands (Modes) 

`interface Management <mgmt-if-id>`

#### Syntax 
```
autoneg <autoneg>
no autoneg
```
#### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| autoneg | on or off  | Select [on(true) off(false) ]  |

## autort 
#### Description 

Auto-derivation of RT 

#### Parent Commands (Modes) 

`address-family l2vpn evpn`

#### Syntax 
```
autort rfc8365-compatible
no autort rfc8365-compatible
```
## bestpath as-path confed 
#### Description 

This command specifies that the length of confederation path sets and
sequences should should be taken into account during the BGP best path
decision process.

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
bestpath as-path confed
no bestpath as-path confed
```
#### Usage Guidelines 

Use this command to consider confederation set and sequence path length
for best-path selection process

#### Examples 
Below command instructs BGP to consider confederation          path length in as-path length comparison during best-path selection process 

```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# bestpath as-path confed
```
## bestpath as-path ignore 
#### Description 

This command influences best-path selection algorithm by not comparing
as-path attribute

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
bestpath as-path ignore
no bestpath as-path ignore
```
#### Usage Guidelines 

Use this command to ignore as-path comparison during best-path selection
process.

#### Examples 
Below command instructs BGP to ignore as-path comparison          during best-path selection process 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# bestpath as-path ignore
```
## bestpath as-path multipath-relax 
#### Description 

This command specifies that BGP decision process should consider paths
of equal AS_PATH length candidates for multipath computation. Without
the knob, the entire AS_PATH must match for multipath computation.

#### Parent Commands (Modes) 

`router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }`

#### Syntax 
```
bestpath as-path multipath-relax [ as-set ]
no bestpath as-path multipath-relax [ as-set ]
```
#### Usage Guidelines 

Use this command to ignore as-path check for paths for the same prefix
making all the paths equal irrespctive of their as-path

#### Examples 
Below command relaxes as-path comparison for multipath          case during best-path selection process 
```
sonic(config)# router bgp 65300
sonic(config-router-bgp)# bestpath as-path multipath-relax
```
## bestpath compare-routerid 
$$$
#### Description 
```
This command influences best-path selection algorithm by comparing
router-ids for identical eBGP routes
Ensure that when comparing routes where both are equal on most metrics,
including local-pref, AS_PATH length, IGP cost, MED, that the tie is
broken based on router-ID.
If this option is enabled, then the already-selected check, where
already selected eBGP routes are preferred, is skipped.
If a route has an ORIGINATOR_ID attribute because it has been reflected,
that ORIGINATOR_ID will be used. Otherwise, the router-ID of the peer
the route was received from will be used.
The advantage of this is that the route-selection (at this point) will
be more deterministic. The disadvantage is that a few or even one
lowest-ID router may attract all traffic to otherwise-equal paths
because of this check. It may increase the possibility of MED or IGP
oscillation, unless other measures were taken to avoid these. The exact
behaviour will be sensitive to the iBGP and reflection topology.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
bestpath compare-routerid
no bestpath compare-routerid
```
### Usage Guidelines 
```
Use this command to compare router-ids as tie-breaker for identical
eBGP paths
```
### Examples 
#### Below command instructs BGP to compare router-ids for          identical eBGP paths 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# bestpath compare-routerid
```
## bestpath med 
### Description 
```
This command influences best-path selection algorithm by how missing
MEDs are treated as well as whether MEDs should be compared for
confederation paths.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
bestpath med { { missing-as-worst [ confed ] } | { confed [ missing-as-worst ] } }
no bestpath med { { [ missing-as-worst ] [ confed ] } | { [ confed ] [ missing-as-worst ] } }
```
### Usage Guidelines 
```
Use this command to consider MED for confederation paths for best-path
selection process. Also, if MED is missing, should it be considered as
worst MED.
```
### Examples 
#### Below command instructs BGP to consider missing MED as          worst and compare MED value for confederation paths 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# bestpath med missing-as-worst confed
```
## bfd 

### Description 

```
Configure BFD peers 


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
bfd

```
## bfd 
### Description 
```
This command enables BFD liveliness check for a BGP neighbor
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
bfd [ check-control-plane-failure ]
no bfd [ check-control-plane-failure ]
```
### Usage Guidelines 
```
Use this command to enable BFD for a BGP neighbor.
check-control-plane-failure links Data Plane status to the BGP control
control plane
```
### Examples 
#### Following command enables BFD for BGP neighbor          30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# bfd
```
## bfd 
### Description 
```
This command enables BFD liveliness check for BGP neighbors in a
peer-group
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
bfd [ check-control-plane-failure ]
no bfd [ check-control-plane-failure ]
```
### Usage Guidelines 
```
Use this command to enable BFD for a BGP peer-group.
check-control-plane-failure links Data Plane status to the BGP control
control plane
```
### Examples 
#### Following command enables BFD for BGP peer-group          PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# bfd
```
## bgp as-path-list 
### Description 
```
This command creates BGP AS Path list
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
bgp as-path-list <as-path-list-name> { regex { <regx-id> { [ any ] | [ all ] } } }
no bgp as-path-list <as-path-list-name> { [ regex ] <regx-id> }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-path-list-name | String  | String  |
| regx-id | String  | String  |
### Usage Guidelines 
```
Use this command to create BGP AS Path list. User can enter a regular
expression of AS Paths that provides flexible and powerful match
support. The command also provides any and all options to allow matching
all or any entry in as-path-list
```
### Examples 
#### The following command creates two entries for a as-path list named          asp_private 
```
sonic# configure terminal
sonic(config)# bgp as-path-list asp_private regex ^65000.*6510565109$
sonic(config)# bgp as-path-list asp_private regex 65107.*65200
```
## bgp community-list 
### Description 
```
This command creates BGP community list
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
bgp community-list { { standard { <community-list-name> { { <aann> [ local-AS ] [ no-advertise ] [ no-export ] [ no-peer ] { [ any ] | [ all ] } } | { local-AS [ <aann> ] [ no-advertise ] [ no-export ] [ no-peer ] { [ any ] | [ all ] } } | { no-advertise [ <aann> ] [ local-AS ] [ no-export ] [ no-peer ] { [ any ] | [ all ] } } | { no-export [ <aann> ] [ local-AS ] [ no-advertise ] [ no-peer ] { [ any ] | [ all ] } } | { no-peer [ <aann> ] [ local-AS ] [ no-advertise ] [ no-export ] { [ any ] | [ all ] } } } } } | { expanded { <community-expanded-list-name> { <line> { [ any ] | [ all ] } } } } }
no bgp community-list { { standard { <community-list-name> { [ <aann> ] | [ local-AS ] | [ no-advertise ] | [ no-export ] | [ no-peer ] } } } | { expanded { <community-expanded-list-name> [ <line> ] } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| community-list-name | String  | String  |
| aann | AA:NN  | String  |
| community-expanded-list-name | String  | String  |
| line | Line  | String  |
### Usage Guidelines 
```
Use this command to create BGP community list. The command provides
options to create expanded or standard community and accepts community
in AA:NN, IP:NN and well-known communities format. This command also
provides any and all constructs to enable user to design community
filters with clause match any or all. For expanded community, user can
specify a regular expression of communities.
```
### Examples 
#### The following command creates a community list named          CommList_RT 
```
sonic# configure terminal
sonic(config)# bgp community-list standard CommList_RT 100:200
sonic(config)# bgp community-list standard CommList_RT no-export
sonic(config)# bgp community-list standard CommList_RT no-peer
sonic(config)# bgp community-list standard CommList_RT 65100:3456
```
## bgp extcommunity-list 
### Description 
```
This command creates BGP extended community list entries
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
bgp extcommunity-list { { standard { <extcommunity-list-name> { { rt { <aa> | <ipaddrnn> } { [ any ] | [ all ] } } | { soo { <aa> | <ipaddrnn> } { [ any ] | [ all ] } } } } } | { expanded { <extcommunity-list-name> { <line> { [ any ] | [ all ] } } } } }
no bgp extcommunity-list { { standard { <extcommunity-list-name> { { [ rt ] { <aa> | <ipaddrnn> } } | { [ soo ] { <aa> | <ipaddrnn> } } } } } | { expanded { <extcommunity-list-name> [ <line> ] } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| extcommunity-list-name | String  | String  |
| aa | AA:NN  | String  |
| ipaddrnn | A.B.C.D:[1..65535]  | String  |
| line | Line  | String  |
### Usage Guidelines 
```
Use this command to create BGP extended community list entries. The command provides
options to create expanded or standard extended community list entries.
For standard extended community, user can create rt or soo type of
communities and command will accept communities in AA:NN or IP:NN
formats. For expanded extended community, the command will accept a
regular expression of communities, which is very flexible and powerful
for matching communities in routes. This command also provides option
for matching all or any extended communities.
```
### Examples 
#### The following command creates netries in a extended community list named          ExtComm_AllowInt 
```
sonic# configure terminal
sonic(config)# bgp extcommunity-list standard ExtComm_AllowInt rt 19.32.56.167:65011 all
sonic(config)# bgp extcommunity-list standard ExtComm_AllowInt rt 31.67.182.214:3001 all
sonic(config)# bgp extcommunity-list standard ExtComm_AllowInt soo 4001:65010 all
sonic(config)# bgp extcommunity-list standard ExtComm_AllowInt soo 98.13.175.21:65101 all
```
## binding 
### Description 
```
Create binding between an ACL and a NAT pool 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
binding <binding-name> <pool-name> [ <acl-name> ] [ <natType> ] [ twice-nat-id ] <twice-nat-id-value>
no binding <bind-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| binding-name | String  | String  |
| pool-name | String  | String  |
| acl-name | String  | String  |
| natType | NAT type  | Select [snat dnat ]  |
| twice-nat-id-value | Unsigned integer  | String  |
## call 
### Description 
```
Jump to another Route-Map after match_set 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
call <match-call>
no call
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-call | String  | String  |
## capability dynamic 
### Description 
```
This command allows bgp to advertise dynamic capability to a neighbor
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
capability dynamic
no capability dynamic
```
### Usage Guidelines 
```
Use this command to turn on dynamic capability for a BGP neighbor
```
### Examples 
#### Following command enables dynamic capability           for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# capability dynamic
```
## capability dynamic 
### Description 
```
This command allows bgp to advertise dynamic capability to neighbors in
a peer-group
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
capability dynamic
no capability dynamic
```
### Usage Guidelines 
```
Use this command to turn on dynamic capability for a BGP peer-group
```
### Examples 
#### Following command enables dynamic capability           for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# capability dynamic
```
## capability extended-nexthop 
### Description 
```
This command allows bgp to negotiate the extended-nexthop capability with
it's peer. If you are peering over a v6 LL address then this capability
is turned on automatically. If you are peering over a v6 Global Address
then turning on this command will allow BGP to install v4 routes with v6
nexthops if you do not have v4 configured on interfaces.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
capability extended-nexthop
no capability extended-nexthop
```
### Usage Guidelines 
```
Use this command to turn on extended-nexthop capability for a BGP
neighbor
```
### Examples 
#### Following command enables extended-nexthop capability           for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# capability extended-nexthop
```
## capability extended-nexthop 
### Description 
```
This command allows bgp to negotiate the extended-nexthop capability with
it's peer in a peer-group. If you are peering over a v6 LL address then
this capability is turned on automatically. If you are peering over a v6
Global Address then turning on this command will allow BGP to install v4
routes with v6 nexthops if you do not have v4 configured on interfaces.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
capability extended-nexthop
no capability extended-nexthop
```
### Usage Guidelines 
```
Use this command to turn on extended-nexthop capability for a BGP
peer-group
```
### Examples 
#### Following command enables extended-nexthop capability           for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# capability extended-nexthop
```
## capability orf prefix-list 
### Description 
```
This command enables BGP to advertise Outbound Route Filtering (ORF) capability
to this neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
### Usage Guidelines 
```
Use this command to advertise Outbound Route Filtering capability to
neighbor. This capability can be enabled in inbound and outbound
direction separately
```
### Examples 
#### Following command enables BGP to advertise ORF          capability to neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# capability orf prefix-list send
```
## capability orf prefix-list 
### Description 
```
This command enables BGP to advertise Outbound Route Filtering (ORF) capability
to neighbors in a peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
### Usage Guidelines 
```
Use this command to advertise Outbound Route Filtering capability to
neighbors in a peer-group. This capability can be enabled in inbound
and outbound direction separately
```
### Examples 
#### Following command enables BGP to advertise ORF          capability to neighbors in a peer-group 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# capability orf prefix-list send
```
## capability orf prefix-list 
### Description 
```
Advertise prefixlist ORF capability to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
## capability orf prefix-list 
### Description 
```
Advertise capability to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
## capability orf prefix-list 
### Description 
```
Advertise prefixlist ORF capability to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
## capability orf prefix-list 
### Description 
```
Advertise capability to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
capability orf prefix-list { send | receive | both }
no capability orf prefix-list { [ send ] | [ receive ] | [ both ] }
```
## channel-group 
### Description 
```
Configure PortChannel parameters 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
channel-group <lag-id>
no channel-group
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| lag-id |   | Integer  |
## clear bgp l2vpn evpn 

### Description 

```
Address family modifier 


```
### Syntax 

```
clear bgp l2vpn evpn { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv6> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ <neighbor-ipv4> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-num-dot | 1-4294967295  | Integer  |
| ifname | String  | String  |
| peer-group name | String  | String  |
| neighbor-ipv6 | A::B  | String  |
| neighbor-ipv4 | A.B.C.D  | String  |


## clear counters 

### Description 

```
Clear counters 


```
### Syntax 

```
clear counters interface { all | { Ethernet [ <ifId> ] } | { PortChannel [ <ifId> ] } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ifId | String  | String  |


## clear ip arp 

### Description 

```
clear ARP commands 


```
### Syntax 

```
clear ip arp [ <ip-addr> ] [ force ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A.B.C.D  | String  |


## clear ip arp interface 

### Description 

```
clear ARP entries for this interface 


```
### Syntax 

```
clear ip arp interface <if-type> <if-id> [ force ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| if-type | Interface type  | Select [Ethernet Vlan PortChannel Management(eth) ]  |
| if-id | Unsigned integer  | String  |


## clear ip bgp 

### Description 

```
This command clears/resets BGP information including neighbors,
peer-group etc.


```
### Syntax 

```
clear ip bgp { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv4> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip4> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv6> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip6> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { ipv4 { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv4> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip4> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { ipv6 { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv6> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip6> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ vrf ] { <vrf-name> { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv4> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip4> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv6> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip6> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { ipv4 { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv4> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip4> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { ipv6 { { [ <as-num-dot> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ * ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ external ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ interface ] { <ifname> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ peer-group ] { <peer-group name> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | { [ <neighbor-ipv6> ] { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } | { [ prefix ] { <prefix-ip6> { [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } | [ in ] | [ out ] | { [ soft ] [ in ] [ out ] } } } } } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-num-dot | 1-4294967295  | Integer  |
| ifname | String  | String  |
| peer-group name | String  | String  |
| neighbor-ipv4 | A.B.C.D  | String  |
| prefix-ip4 | A.B.C.D/mask  | String  |
| neighbor-ipv6 | A::B  | String  |
| prefix-ip6 | A::B/mask  | String  |
| vrf-name | String(Max: 15 characters)  | String  |


### Usage Guidelines 

```
Use this command to clear BGP information. Following is a partial list of
information with command syntax that can be cleared.
- clear ip bgp *
  This command clears all BGP neighbors
- clear ip bgp {ipv4 | ipv6} unicast *
  This command clears all BGP neighbors with this address-family and
  sub-address-family activated
- clear ip bgp {ipv4 | ipv6} peer_ip *
  Clear peers with address of peer_ip and this address-family activated.
- clear ip bgp {ipv6 | ipv4} soft {in | out}
  'in" option will send route-refresh request unless using 'soft-reconfiguration inbound.
  'out' option will resend all outbound updates


```
### Examples 
#### Below command resets a BGP neighbor 14.14.14.1 

```
leaf4# clear ip bgp 14.14.14.1


```
## clear ipv6 neighbors 

### Description 

```
clear NDP commands 


```
### Syntax 

```
clear ipv6 neighbors [ <ip-addr> ] [ force ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A::B  | String  |


## clear ipv6 neighbors interface 

### Description 

```
clear NDP entries for this interface 


```
### Syntax 

```
clear ipv6 neighbors interface <if-type> <if-id> [ force ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| if-type | Interface type  | Select [Ethernet Vlan PortChannel Management(eth) ]  |
| if-id | Unsigned integer  | String  |


## clear mac address-table dynamic 

### Description 

```
Clear MAC address-table for dynamic commands 


```
### Syntax 

```
clear mac address-table dynamic { all | { address <mac-addr> } | { Vlan <vlan-id> } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |
| vlan-id |   | Integer  |


## clear nat 

### Description 

```
Clear NAT 


```
### Syntax 

```
clear nat { translations | statistics }

```
## client-to-client reflection 
### Description 
```
This command configures client to client route reflection
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
client-to-client reflection
no client-to-client reflection
```
### Usage Guidelines 
```
Use this comand to configure client to client route reflection
```
### Examples 
#### Below command configures client to client reflection 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# client-to-client reflection
```
## cluster-id 
### Description 
```
This command configures cluster ID for BGP router
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
cluster-id <intval-ip>
no cluster-id
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| intval-ip | A.B.C.D or [1..4294967295]  | String  |
### Usage Guidelines 
```
A cluster is a collection of route reflectors and their clients, and is
used by route reflectors to avoid looping. Use this command to configure
cluster-ID (an IP address or a number) on a BGP router
```
### Examples 
#### Below command configures cluster ID 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# cluster-id 23.79.154.17
```
## coalesce-time 
### Description 
```
This command configures subgroup coalesce timer interval in millseconds
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
coalesce-time <coaltime>
no coalesce-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| coaltime | 1-4294967295  | Integer  |
### Usage Guidelines 
```
Use this command to configure subgroup coalesce timer interval
```
### Examples 
#### Below command configures the coalesce timer interval to          2000 msec 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# coalesce-time 2000
```
## collector 
### Description 
```
This command is used to configure the external collector IP address and port.
Report will be forwarded to the collector accordingly.
```
### Parent Commands (Modes) 
```
tam
```
### Syntax 
```
collector <name> type <ip-type-val> ip <ip-addr-val> port <port-val>
no collector <name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |
| ip-type-val |   | Select [ipv4(ipv4) ipv6(ipv6) ]  |
| ip-addr-val | A.B.C.D/A::B  | String  |
| port-val |   | Integer  |
### Usage Guidelines 
```
Reports are sent by the configured external collector by the silicon.
```
### Examples 
#### Configure TAM collector 
```
sonic(config-tam)# collector c1 type ipv4 ip 3.3.3.3 port 7777
```
## confederation 
### Description 
```
This command configures the list of AS numbers that are part of the
confederation. This command also allows user to configure configure the
router's confederation ID
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
confederation { { identifier <id-as> } | { peers <peer-as> } }
no confederation { { identifier <id-as> } | peers }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| id-as | 1-4294967295  | Integer  |
| peer-as | 1-4294967295  | Integer  |
### Usage Guidelines 
```
Use this command to create confederation peers and local confederation
Id
```
### Examples 
#### Below command configures local confederation Id and          creates confederation peers 
```
         sonic# configure terminal
         sonic(config)# router bgp 65300
         sonic(config-router-bgp)# confederation identifier 65000
         sonic(config-router-bgp)# confederation peers 65100
         sonic(config-router-bgp)# confederation peers 65200
         sonic(config-router-bgp)# confederation peers 65300
```
## configure terminal 

### Description 

```
Configure from the terminal 


```
### Syntax 

```
configure terminal

```
## copy 

### Description 

```
Perform file copy operations 


```
### Syntax 

```
copy { { <copy_config_url> { running-configuration [ overwrite ] } } | { running-configuration <filepath> } | { startup-configuration { running-configuration [ overwrite ] } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| copy_config_url | file:  | String  |
| filepath | file:  | String  |


## dampening 
### Description 
```
This command enables BGP route-flap dampening and specifies dampening
parameters
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
dampening [ <halflife> ] { [ <reusethr> ] { <suppressthr> <maxsuppress> } }
no dampening
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| halflife |   | Integer  |
| reusethr |   | Integer  |
| suppressthr |   | Integer  |
| maxsuppress |   | Integer  |
### Usage Guidelines 
```
Use this command to configure route flap dampening feature for BGP
routes. Route flap dampening algorithm is compatible with RFC 2439. The
use of this command is not recommended nowadays. Currently
implementation works only for IPv4 address family
```
### Examples 
#### The below configuration example enables route-flap          dampeninmg feature 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# dampening 10 1200 2000 40
```
## default ipv4-unicast 
### Description 
```
This command activate IPv4 unicast address-family for a BGP peer by
default
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
default ipv4-unicast
no default ipv4-unicast
```
### Usage Guidelines 
```
Use this command to activate IPv4 unicast address family on BGP
neighbors by default
```
### Examples 
#### Below command enables IPv4 unicast address family on all          BGP neighbors by default 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# default ipv4-unicast
```
## default local-preference 
### Description 
```
This command the default value for Local Preference parameter
default
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
default local-preference <lprftime>
no default local-preference
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| lprftime |   | Integer  |
### Usage Guidelines 
```
Use this command to set the deafult value of Local Preference parameter
```
### Examples 
#### Below command sets default local preference to 200 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# default local-preference 200
```
## default show-hostname 
### Description 
```
This command instructs BGP to display hostname in certain display
commands
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
default show-hostname
no default show-hostname
```
### Usage Guidelines 
```
Use this command to instruct BGP to display hostname in certain display
command outputs.
```
### Examples 
#### Below command sets BGP to display hostname in certain          display commands 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# default show-hostname
```
## default shutdown 
### Description 
```
This command instructs BGP to make newly created neighbors in shutdown
state
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
default shutdown
no default shutdown
```
### Usage Guidelines 
```
By default, newly created BGP neighbors are in admin enabled state. Use
this command to keep newly created BGP neighbors in admin shutdown
state.
```
### Examples 
#### Below command configures BGP to keep newly created          neighbors in shutdown state 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# default shutdown
```
## default subgroup-pkt-queue-max 
### Description 
```
This command configures the maximum packet queue length for update
groups
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
default subgroup-pkt-queue-max <maxval>
no default subgroup-pkt-queue-max
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| maxval |   | Integer  |
### Usage Guidelines 
```
Use this command to set a default maximum packet queue length for update
groups
```
### Examples 
#### Below command configures maximum packet queue length to          50 for update groups 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# default subgroup-pkt-queue-max 50
```
## default-originate 
### Description 
```
This command enables BGP to originate default route to this neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
### Usage Guidelines 
```
Use this command to originate a default route to this neighbor. User can
optionally use route-map along with this command to to specify criteria
to originate default
```
### Examples 
#### Following command enables BGP to originate a default          route to neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# default-originate
```
## default-originate 
### Description 
```
This command enables BGP to originate default route to neighbors in a
peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
### Usage Guidelines 
```
Use this command to originate default route to neighbors in a peer-group. User can
optionally use route-map along with this command to to specify criteria
to originate default
```
### Examples 
#### Following command enables BGP to originate default          route to neighbors in peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# default-originate
```
## default-originate 
### Description 
```
Originate default route to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
## default-originate 
### Description 
```
Originate default route to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
## default-originate 
### Description 
```
Originate default route to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
## default-originate 
### Description 
```
Originate default route to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
default-originate [ route-map ] <rtemap>
no default-originate [ route-map ] <rtemap>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtemap | String  | String  |
## default-originate ipv4 
### Description 
```
Address family IPv4 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
default-originate ipv4
no default-originate ipv4
```
## default-originate ipv6 
### Description 
```
Address family IPv6 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
default-originate ipv6
no default-originate ipv6
```
## description 
### Description 
```
This command configures a display string for a BGP neighbor
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
description <String>
no description [ <String> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| String | String  | String  |
### Usage Guidelines 
```
Use this command to configure a descriptive string for a BGP neighbor
```
### Examples 
#### Following command configures description for BGP          neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# remote-as 65100
sonic(config-router-bgp-neighbor)# description to_nyc_dc1
```
## description 
### Description 
```
This command configures a display string for a BGP peer-group
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
description <String>
no description [ <String> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| String | String  | String  |
### Usage Guidelines 
```
Use this command to configure a descriptive string for a BGP peer-group
```
### Examples 
#### Following command configures description for BGP          peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# description My_PG_East_Cost_Nbrs
```
## description 
### Description 
```
Textual description 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
description <desc>
no description
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| desc | String  | String  |
## description 
### Description 
```
Textual description 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
description <desc>
no description
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| desc | String  | String  |
## description 
### Description 
```
Description of the group (Max size 255) 
```
### Parent Commands (Modes) 
```
link state track <grp-name>
```
### Syntax 
```
description <grp-descr>
no description
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-descr | String  | String  |
## destination 

### Description 

```
Configure ERSPAN/SPAN mirror session


```
### Parent Commands (Modes) 

```
mirror-session <session-name>

```
### Syntax 

```
destination <phy-if-id> [ source ] <src-phy-if-id> [ direction ] <sess-direction> [ dst-ip ] <dst_ip> [ src-ip ] <src_ip> [ dscp ] <ip_dscp> [ gre ] <ip_gre> [ ttl ] <ip_ttl> [ queue ] <queue_val>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-id | String  | String  |
| src-phy-if-id | String  | String  |
| sess-direction | Port mirror session direction  | Select [rx(rx) tx(tx) both(both) ]  |
| dst_ip | A.B.C.D  | String  |
| src_ip | A.B.C.D  | String  |
| ip_dscp |   | Integer  |
| ip_gre | Hexadecimal Type  | String  |
| ip_ttl |   | Integer  |
| queue_val |   | Integer  |


### Examples 

```
sonic(config)# mirror-session Mirror1
sonic(config-mirror-Mirror1)# destination Ethernet0 source Ethernet4 direction rx
Success
sonic(config-mirror-Mirror1)# exit
sonic(config)# mirror-session Mirror2
sonic(config-mirror-Mirror2)# destination erspan dst-ip 10.1.1.1 src-ip 11.1.1.1 dscp 10 ttl 10 gre 0x88ee queue 10 source Ethernet4 direction rx
Success
sonic(config-mirror-Mirror2)#


```
## detect-multiplier 

### Description 

```
Configure detection multiplier for Bidirectional Forwarding detection(BFD) peer for timeout.


```
### Parent Commands (Modes) 

```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>

```
### Syntax 

```
detect-multiplier <multiplier>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| multiplier |   | Integer  |


### Usage Guidelines 

```
Default value is 3.


```
### Examples 
#### Configure detection multiplier 

```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# detect-multiplier 5


```
## deterministic-med 
### Description 
```
This command enables to carry out route-selection in a way that produces
deterministic results locally, even in the face of MED and the lack of a
well-defined order of preference it can induce on routes.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
deterministic-med
no deterministic-med
```
### Usage Guidelines 
```
Carry out route-selection in a way that produces deterministic answers
locally, even in the face of MED and the lack of a well-defined order of
preference it can induce on routes. Without this option the preferred
route with MED may be determined largely by the order that routes were
received in.
Setting this option will have a performance cost that may be noticeable
when there are many routes for each destination. Currently in BGP it is
implemented in a way that scales poorly as the number of routes per
destination increases.
By default deterministic-med is disabled
```
### Examples 
#### Below command enables deterministics-med 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# deterministic-med
```
## device-id 
### Description 
```
This command is used to configure the deviceId of the switch. Last 23 bits of mac-address are used as default deviceId
```
### Parent Commands (Modes) 
```
tam
```
### Syntax 
```
device-id <device-id>
no device-id
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| device-id |   | Integer  |
### Usage Guidelines 
```
This command is used to configure the device identifier of the switch
```
### Examples 
#### Configure device-id 
```
sonic(config-tam)# device-id 5000
```
## disable-connected-check 
### Description 
```
This command disables the restriction that eBGP peers must be directly
connected
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
disable-connected-check
no disable-connected-check
```
### Usage Guidelines 
```
Use this command to allow peerings between directly connected eBGP peers
using loopback addresses.
```
### Examples 
#### Following command disables connected check           for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# disable-connected-check
```
## disable-connected-check 
### Description 
```
This command disables the restriction that eBGP peers must be directly
connected
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
disable-connected-check
no disable-connected-check
```
### Usage Guidelines 
```
Use this command to allow peerings between directly connected eBGP peers
using loopback addresses.
```
### Examples 
#### Following command disables connected check           for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# disable-connected-check
```
## disable-ebgp-connected-route-check 
### Description 
```
This command disables eBGP connected route check
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
disable-ebgp-connected-route-check
no disable-ebgp-connected-route-check
```
### Usage Guidelines 
```
Use this command to disable checking if next-hop is conencted on ebgp
sessions. When BGP peering is between the loopback interfaces, user
should enable this option.
```
### Examples 
#### Below command disables eBGP connected route check 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# disable-ebgp-connected-route-check
```
## distance bgp 
### Description 
```
This command changes distance value of BGP. The command allows finer
control to change the distance values for external routes, internal
routes and local routes separately
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
distance bgp <external> { <internal> <local> }
no distance bgp
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| external |   | Integer  |
| internal |   | Integer  |
| local |   | Integer  |
### Usage Guidelines 
```
Use this command to configure administrative distance for BGP route
types
```
### Examples 
#### This configuration example sets administrative distance          of 100, 50 and 10 for external, internal and local BGP routes          respectively under ipv4 address-family 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# distance bgp 100 50 10
```
## distance bgp 
### Description 
```
Define an administrative distance 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
distance bgp <external> { <internal> <local> }
no distance bgp
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| external |   | Integer  |
| internal |   | Integer  |
| local |   | Integer  |
## dont-capability-negotiate 
### Description 
```
This command suppresses sending Capability Negotiation as OPEN message
optional parameter to the peer. This command only affects the peer is
configured other than IPv4 unicast configuration.
When remote peer does not have capability negotiation feature, remote
peer will not send any capabilities at all. In that case, bgp configures
the peer with configured capabilities.
You may prefer locally configured capabilities more than the negotiated
capabilities even though remote peer sends capabilities. If the peer is
configured by override-capability, BGP ignores received capabilities
then override negotiated capabilities with configured values.
Additionally the user should be reminded that this feature
fundamentally disables the ability to use widely deployed BGP features -
BGP unnumbered, hostname support, AS4, Addpath, Route Refresh, ORF,
Dynamic Capabilities, and graceful restart.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
dont-capability-negotiate
no dont-capability-negotiate
```
### Usage Guidelines 
```
Use this command to disable capability negotiation for a BGP neighbor
```
### Examples 
#### Following command disables capability negotiation            for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# dont-capability-negotiate
```
## dont-capability-negotiate 
### Description 
```
This command suppresses sending Capability Negotiation as OPEN message
optional parameter to neighbors in a peer-group. This command only
affects the peer is configured other than IPv4 unicast configuration.
When remote peer does not have capability negotiation feature, remote
peer will not send any capabilities at all. In that case, bgp configures
the peer with configured capabilities.
You may prefer locally configured capabilities more than the negotiated
capabilities even though remote peer sends capabilities. If the peer is
configured by override-capability, BGP ignores received capabilities
then override negotiated capabilities with configured values.
Additionally the user should be reminded that this feature
fundamentally disables the ability to use widely deployed BGP features -
BGP unnumbered, hostname support, AS4, Addpath, Route Refresh, ORF,
Dynamic Capabilities, and graceful restart.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
dont-capability-negotiate
no dont-capability-negotiate
```
### Usage Guidelines 
```
Use this command to disable capability negotiation for BGP neighbors in
a peer-group
```
### Examples 
#### Following command disables capability negotiation            for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# dont-capability-negotiate
```
## downstream 
### Description 
```
Set downstream ports 
```
### Parent Commands (Modes) 
```
link state track <grp-name>
```
### Syntax 
```
downstream all-mclag
no downstream all-mclag
```
## drop-monitor 

### Description 

```
TAM DROP MONITOR configuration 


```
### Parent Commands (Modes) 

```
tam

```
### Syntax 

```
drop-monitor

```
## dup-addr-detection 
### Description 
```
Duplicate address detection 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
dup-addr-detection [ max-moves ] { <nummoves> { time <timevalue> } }
no dup-addr-detection [ max-moves ] { <nummoves> { time <timevalue> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| nummoves | Number of moves 2-1000, default 5  | Integer  |
| timevalue | Time in seconds 2-1800, default 180  | Integer  |
## dup-addr-detection freeze 
### Description 
```
Duplicate address detection freeze 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
dup-addr-detection freeze { permanent | <time> }
no dup-addr-detection freeze { permanent | <time> }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| time | Time in seconds 30-3600, default 180  | Integer  |
## ebgp-multihop 
### Description 
```
This command enable multihop attribute for EBGP neighbors
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
ebgp-multihop [ <hop-count> ]
no ebgp-multihop [ <hop-count> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| hop-count |   | Integer  |
### Usage Guidelines 
```
EBGP neighbors that are multiple hops away need this configuration. User
can optionally set the maximum hops that BGP neighbors can be apart.
```
### Examples 
#### Following command configures ebgp-multihop for neighbor          30.30.30.3 with maximum hops = 10 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# remote-as 65100
sonic(config-router-bgp-neighbor)# ebgp-multihop 10
```
## ebgp-multihop 
### Description 
```
This command enables multihop for EBGP peer-group
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
ebgp-multihop [ <hop-count> ]
no ebgp-multihop [ <hop-count> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| hop-count |   | Integer  |
### Usage Guidelines 
```
peer-group with eBGP neighbors as members that are multiple hops away
need this configuration. User can optionally set the maximum hops that
BGP neighbors in peer-group can be apart.
```
### Examples 
#### Following command configures ebgp-mltihop for peer-group          PG_Ext with max hop = 10 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# ebgp-multihop 10
```
## echo-interval 

### Description 

```
Configure desired echo packet transmit interval for Bidirectional Forwarding detection(BFD) peer.


```
### Parent Commands (Modes) 

```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>

```
### Syntax 

```
echo-interval <echo_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| echo_interval |   | Integer  |


### Usage Guidelines 

```
Default value is 50 milliseconds.


```
### Examples 
#### Configure packet echo transmit interval 

```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# echo-interval 200


```
## echo-mode 
### Description 
```
Enable echo-mode for Bidirectional Forwarding detection(BFD) peer.
```
### Parent Commands (Modes) 
```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>
```
### Syntax 
```
echo-mode
no echo-mode
```
### Usage Guidelines 
```
This command can be used to enable echo mode for BFD single-hop peer, echo mode is not supported for multi-hop peers.
```
### Examples 
#### Enable echo mode 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# echo-mode
```
## enable 
### Description 
```
Enable NAT feature 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
enable
no enable
```
## enforce-first-as 
### Description 
```
This command enforces that first AS in as-path of a route received from
BGP peer must be peer's AS number
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
enforce-first-as
no enforce-first-as
```
### Usage Guidelines 
```
Use this command to enforce that first AS in as-path of route from eBGP
peer must be peer's local AS number
```
### Examples 
#### Following command enables enforcement of first AS number            for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# enforce-first-as
```
## enforce-first-as 
### Description 
```
This command enforces that first AS in as-path of a route received from
BGP peer must be peer's AS number
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
enforce-first-as
no enforce-first-as
```
### Usage Guidelines 
```
Use this command to enforce that first AS in as-path of route from eBGP
peer must be peer's local AS number
```
### Examples 
#### Following command enables enforcement of first AS number            for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# enforce-first-as
```
## enforce-multihop 
### Description 
```
This command enforces that eBGP neighbors perform multihop
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
enforce-multihop
no enforce-multihop
```
### Usage Guidelines 
```
Use this command to enforce eBGP neighbors perform multihop
```
### Examples 
#### Following command enables enforce-multihop           for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# enforce-multihop
```
## enforce-multihop 
### Description 
```
This command enforces that eBGP neighbors in a peer-group perform multihop
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
enforce-multihop
no enforce-multihop
```
### Usage Guidelines 
```
Use this command to enforce eBGP neighbors in a peer-group perform multihop
```
### Examples 
#### Following command enables enforce-multihop           for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# enforce-multihop
```
## evpn 

### Description 

```
Command to enter EVPN configuration mode.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
evpn <evpn_name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| evpn_name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
(config)# evpn NVONAME
NVONAME - string


```
### Examples 
#### configuration mode for evpn 

```
sonic(config)# evpn evpn1
sonic(conf-if-evpn)#


```
## fast-external-failover 
### Description 
```
This command causes bgp to take down ebgp peers immediately when a
link flaps.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
fast-external-failover
no fast-external-failover
```
### Usage Guidelines 
```
Use this command to control how sensitive eBGP neighborship is to the
underlying link failure.
```
### Examples 
#### Below command enables fast external failover feature for          BGP neighbors 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# fast-external-failover
```
## feature 

### Description 

```
This command is used to enable/disable the drop monitor feature functionality.


```
### Parent Commands (Modes) 

```
drop-monitor

```
### Syntax 

```
feature { enable | disable }

```
### Usage Guidelines 

```
This command is used to enable/disable the drop monitor feature functionality.


```
### Examples 
#### Enable or Disable Drop-Monitor Feature 

```
sonic(config-drop-monitor)# feature enable
sonic(config-drop-monitor)# feature disable


```
## feature 

### Description 

```
Enables or disables IFA feature.


```
### Parent Commands (Modes) 

```
int-ifa

```
### Syntax 

```
feature <enable>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| enable | enable or disable  | Select [enable(enable) disable(disable) ]  |


### Usage Guidelines 

```
Use this command to enable or disable IFA feature.


```
### Examples 
#### Enable or Disable IFA 

```
sonic(config-tam-int-ifa)# feature disable

sonic(config-tam-int-ifa)# do show tam int-ifa supported
---------------------------------------------------------
TAM IFA Feature Information
---------------------------------------------------------
IFA Feature Supported: False


```
## feature 

### Description 

```
Enable or disable IFA Tail Timestamping feature.


```
### Parent Commands (Modes) 

```
int-ifa-ts

```
### Syntax 

```
feature { enable | disable }

```
### Usage Guidelines 

```
Use this command to enable or disable IFA Tail Timestamping feature.


```
### Examples 
#### Enable/disable IFA Tail Timestamping feature 

```
dhcp-10-59-142-164(config-int-ifa-ts)# feature enable
dhcp-10-59-142-164(config-int-ifa-ts)#


```
## filter-list 
### Description 
```
This command configures a filter list for a BGP neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
### Usage Guidelines 
```
Use this command to define policy (route filtering) for a BGP neighbor
in outbound or/and inbound direction.
```
### Examples 
#### Following command configures a filter-list          fl_allow_remote in inbound direction for neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# filter-list fl_allow_remote in
```
## filter-list 
### Description 
```
This command configures a filter list for BGP peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
### Usage Guidelines 
```
Use this command to define policy (route filtering) for a BGP peer-group
in outbound or/and inbound direction.
```
### Examples 
#### Following command configures a filter-list          fl_allow_remote in inbound direction for peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# filter-list fl_allow_remote in
```
## filter-list 
### Description 
```
Establish BGP filters 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
## filter-list 
### Description 
```
Establish BGP filters 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
## filter-list 
### Description 
```
Establish BGP filters 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
## filter-list 
### Description 
```
Establish BGP filters 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
filter-list <fname> { in | out }
no filter-list <fname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| fname | String  | String  |
## flow 
### Description 
```
This command is used to configure a drop-monitor flow. The CLI command associates a flow configuration (specified by the ACL table and ACL rule) with a collector and sampling configuration.
```
### Parent Commands (Modes) 
```
drop-monitor
```
### Syntax 
```
flow <flow-name> acl-table <acl-table-name> acl-rule <acl-rule-name> collector <collector-name> sample <sampling-name> flowgroup-id <flowgroup_id>
no flow <flow-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| flow-name | String(Max: 63 characters)  | String  |
| acl-table-name | String(Max: 63 characters)  | String  |
| acl-rule-name | String(Max: 63 characters)  | String  |
| collector-name | String(Max: 63 characters)  | String  |
| sampling-name | String(Max: 63 characters)  | String  |
| flowgroup_id |   | Integer  |
### Usage Guidelines 
```
This command associates drop-monitor flow with ACL table, ACL rule, collector and sample configuration.
```
### Examples 
#### Configure flow parameters 
```
sonic(config-drop-monitor)# flow f4 acl-table t4 acl-rule r4 collector c1 sample s1 flowgroup-id 4
```
## flow 
### Description 
```
Configures IFA flow.
```
### Parent Commands (Modes) 
```
int-ifa
```
### Syntax 
```
flow <flow-name> acl-table <acl-table-val> acl-rule <acl-rule-val> [ sampling-rate ] <sampling-rate-val> [ collector-name ] <collector-val>
no flow <name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| flow-name | String(Max: 63 characters)  | String  |
| acl-table-val | String(Max: 63 characters)  | String  |
| acl-rule-val | String(Max: 63 characters)  | String  |
| sampling-rate-val | Unsigned integer  | String  |
| collector-val | String(Max: 63 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure an IFA flow. The collector needs to be configured separately.
```
### Examples 
#### Configure IFA flow configuration 
```
sonic(config-tam-int-ifa)# flow iflow1 acl-table iacl1 acl-rule irule1 sampling-rate 12 collector-name icol
sonic(config-tam-int-ifa)# exit
```
## flow 
### Description 
```
Configure Tail Timestamping flow parameters.
```
### Parent Commands (Modes) 
```
int-ifa-ts
```
### Syntax 
```
flow <flow-name> acl-table <acl-table-name> acl-rule <acl-rule-name>
no flow [ <flow-name> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| flow-name | String(Max: 63 characters)  | String  |
| acl-table-name | String(Max: 63 characters)  | String  |
| acl-rule-name | String(Max: 63 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure Tail Timestamping flow table.
```
### Examples 
#### Tail Timestamping flow configuration 
```
dhcp-10-59-142-164(config-int-ifa-ts)# flow flow32 acl-table tacl1 acl-rule trule1
dhcp-10-59-142-164(config-int-ifa-ts)#
```
## graceful-restart enable 
### Description 
```
This command enables Graceful Restart for an instance of BGP
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
graceful-restart enable
no graceful-restart enable
```
### Usage Guidelines 
```
Use this command to enable BGP Graceful Restart globally in an instance
of BGP. Changing the Graceful restart parameter will talke effect only
on the fly will not take effect immediately. It will require all the
BGP neighbors to be reset to take effect. This is because Graceful Restart
capability must be negotiated with neighbors to make this feature
functional.
```
### Examples 
#### Below command enables Graceful Restart for BGP instance on          default-VRF 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# graceful-restart enable
```
## graceful-restart preserve-fw-state 
### Description 
```
This command instructs BGP to preserve forwarding state during Graceful
Restart for an instance of BGP
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
graceful-restart preserve-fw-state
no graceful-restart preserve-fw-state
```
### Usage Guidelines 
```
Use this command to enable BGP to preserve forwarding state of BGP
during Graceful Restart.
```
### Examples 
#### Below command enables preservation of forwarding state          during Graceful Restart for BGP instance on default-VRF 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# graceful-restart preserve-fw-state
```
## graceful-restart restart-time 
### Description 
```
This command configures restart timer interval for BGP
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
graceful-restart restart-time <restart-time>
no graceful-restart restart-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| restart-time |   | Integer  |
### Usage Guidelines 
```
Use this command to configure BGP restart timer interval in seconds.
This is optional parameter and determines how long peer routers
will wait to delete stale routes before a BGP open message is received.
The default value is 120 seconds.
```
### Examples 
#### Below command configures restart timer interval to          180 seconds for BGP instance on default-VRF 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# graceful-restart restart-time 180
```
## graceful-restart stalepath-time 
### Description 
```
This command configures stale path timer interval for BGP
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
graceful-restart stalepath-time <stalepath-time>
no graceful-restart stalepath-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| stalepath-time |   | Integer  |
### Usage Guidelines 
```
This command is used to set the maximum time to hold on to
the stale paths of a gracefully restarted peer. All stale
paths are deleted after the expiration of this timer. This
is an optional parameter. The default is 360 seconds
```
### Examples 
#### Below command configures stale path timer interval to          300 seconds for BGP instance on default-VRF 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# graceful-restart stalepath-time 300
```
## graceful-shutdown 
### Description 
```
This command enables Graceful shutdown feature
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
graceful-shutdown
no graceful-shutdown
```
### Usage Guidelines 
```
Use this command to gracefully remove a BGP router from service. This
command will instruct BGP to enter into graceful shutdown mode by
resending routes with GSHUT community to all it's neighbors. This will
enable all it's neighbor to route traffic around it so that router can
be taken out of service without impact data forwarding
```
### Examples 
#### Below command disables eBGP connected route check 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# graceful-shutdown
```
## image install 

### Description 

```
Install image 


```
### Syntax 

```
image install <img-path>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| img-path | String  | String  |


## image remove 

### Description 

```
Remove an image  


```
### Syntax 

```
image remove { all | <image> }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| image | String  | String  |


## image set-default 

### Description 

```
Set default boot image 


```
### Syntax 

```
image set-default <img-name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| img-name | String  | String  |


## int-ifa 

### Description 

```
INT IFA Configuration 


```
### Parent Commands (Modes) 

```
tam

```
### Syntax 

```
int-ifa

```
## int-ifa-ts 

### Description 

```
TAM INT IFA TS configuration 


```
### Parent Commands (Modes) 

```
tam

```
### Syntax 

```
int-ifa-ts

```
## interface 

### Description 

```
Select an interface 


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
interface { <phy-if-name> | <vlan-if-name> }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-name |   |   |
| vlan-if-name |   |   |


## interface Loopback 
### Description 
```
Loopback Interface Configuration 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
interface Loopback <lo-id>
no interface Loopback <lo-id>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| lo-id |   | Integer  |
## interface Management 

### Description 

```
Management Interface commands 


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
interface Management <mgmt-if-id>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mgmt-if-id |   | Integer  |


## interface PortChannel 
### Description 
```
Port channel Interface Configuration 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
no interface PortChannel <lag-id>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| lag-id |   | Integer  |
| PoMode | PortChannel Mode  | Select [active on ]  |
| min-links-value |   | Integer  |
## interface Vxlan 

### Description 

```
Command to enter VxLAN configuration mode.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
interface Vxlan <vxlan-if-name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vxlan-if-name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
(config)# interface vxlan VTEPNAME
VTEPNAME - string


```
### Examples 
#### configuration mode for vxlan 

```
sonic(config)# interface vxlan vtep1
sonic(config-if-vtep1)#


```
## ip access-group 
### Description 
```
Specify access control for packets 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
ip access-group <access-list-name> { in | out }
no ip access-group <access-list-name> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| access-list-name | String(Max: 63 characters)  | String  |
## ip access-list 
### Description 
```
Configure IPv4 access-list 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ip access-list <access-list-name>
no ip access-list <access-list-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| access-list-name | String(Max: 63 characters)  | String  |
## ip address 
### Description 
```
IP address 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
ip address <addr>
no ip address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask  | String  |
## ip address 
### Description 
```
IP address 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
ip address <addr> [ gwaddr ] <gw_addr>
no ip address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask  | String  |
| gw_addr | A.B.C.D  | String  |
## ip address 
### Description 
```
IP address 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ip address <addr>
no ip address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask  | String  |
## ip address 
### Description 
```
IP address 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
ip address <addr>
no ip address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask  | String  |
## ip address 
### Description 
```
IP address 
```
### Parent Commands (Modes) 
```
interface Loopback <lo-id>
```
### Syntax 
```
ip address <addr>
no ip address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask  | String  |
## ip anycast-address 
### Description 
```
Configures IPv4 Static Anycast Gateway Address for an Interface.
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ip anycast-address <anycast-addr>
no ip anycast-address <anycast-addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| anycast-addr | A.B.C.D/mask  | String  |
## ip anycast-address 

### Description 

```
Enable/Disable IPv4 Static Anycast Gateway functionality. By default it is enabled.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ip anycast-address { enable | disable }

```
## ip anycast-mac-address 
### Description 
```
Configures MAC address for all the Static Anycast Gateway Addresses on the system.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ip anycast-mac-address <anycast-mac>
no ip anycast-mac-address <anycast-mac>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| anycast-mac | nn:nn:nn:nn:nn:nn  | String  |
## ip igmp 
### Description 
```
Commands to configure or unconfigure IGMP snooping parameters on a VLAN
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ip igmp snooping { [ querier ] | [ fast-leave ] | { [ query-interval ] <query-interval-val> } | { [ last-member-query-interval ] <last-mem-query-interval-val> } | { [ query-max-response-time ] <query-max-response-val> } | { [ version ] <igmps-version-val> } | { [ mrouter ] { interface <mrouter-if-name> } } | { [ static-group ] { <group-addr> { interface <grp-if-name> } } } }
no ip igmp snooping { [ querier ] | [ fast-leave ] | [ query-interval ] | [ last-member-query-interval ] | [ query-max-response-time ] | [ version ] | { [ mrouter ] { interface <mrouter-if-name> } } | { [ static-group ] { <group-addr> { interface <grp-if-name> } } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| query-interval-val | Query Interval value (Default: 125 s)  | Integer  |
| last-mem-query-interval-val | Last Member Query Interval value (Default: 1000 ms)  | Integer  |
| query-max-response-val | Query Reponse Time (Default: 10 s)  | Integer  |
| igmps-version-val | IGMPS version 1 or 2 or 3 (Default: 2)  | Integer  |
| mrouter-if-name | String  | String  |
| group-addr | A.B.C.D  | String  |
| grp-if-name | String  | String  |
### Examples 
#### Enable IGMP Snooping on VLAN 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping
```
#### Disable IGMP Snooping on VLAN 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping
```
#### Enable IGMP querier on VLAN, by default querier is disabled 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping querier
```
#### Disable IGMP querier on VLAN 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping querier
```
#### Enable IGMP fast-leave on VLAN, by default fast-leave is disabled 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping fast-leave
```
#### Disable IGMP fast-leave on VLAN 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping fast-leave
```
#### Configure IGMP query-interval, default interval is 125 seconds, range is from 1 to 18000 seconds 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping query-interval 20
```
#### Unconfigure non-default IGMP query-interval configured, value set to default interval 125 seconds 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping query-interval
```
#### Configure last member query interval, default is 1000ms, the valid range is from 100ms to 25500ms 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping last-member-query-interval 2000
```
#### Unconfigure non-default last member query interval configured, value set to default 1s 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping last-member-query-interval
```
#### Configure max response interval, default is 10s, the valid range is from 1 to 25s 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping query-max-response-time 12
```
#### Unconfigure non-default max response interval configured, value set to default 10s 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping query-max-response-time
```
#### Configure IGMP version, default is Version2, the valid range is from 1 to 3 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping version 3
```
#### Unconfigure non-default IGMP version configured, value set to default Version2 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping version
```
#### Configure static multicast router(mrouter) port 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping mrouter interface Ethernet4
```
#### Unconfigure static multicast router(mrouter) port 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# no ip igmp snooping mrouter interface Ethernet4
```
#### Configure static multicast group 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)# ip igmp snooping static-group 225.0.0.1 interface PortChannel2
```
#### Unconfigure static multicast group 
```
sonic(config)# interface Vlan 200
sonic(conf-if-Vlan200)#no ip igmp snooping static-group 225.0.0.1 interface PortChannel2
```
## ip prefix-list 
### Description 
```
Build a prefix list 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ip prefix-list <prefix-name> { { permit { <ipv4-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } | { deny { <ipv4-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } }
no ip prefix-list <prefix-name> { { [ permit ] { <ipv4-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } | { [ deny ] { <ipv4-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix-name | String  | String  |
| ipv4-prefix | A.B.C.D/mask  | String  |
| ge-min-prefix-length |   | Integer  |
| le-max-prefix-length |   | Integer  |
## ip unnumbered 
### Description 
```
Configure IPv4 unnumbered interface by borrowing IPv4 address from the Donor interface.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
ip unnumbered <donor-interface>
no ip unnumbered
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| donor-interface | String  | String  |
### Usage Guidelines 
```
Use this command to configure IPv4 unnumbered interface at the interface level.
```
### Examples 
#### Configure IPv4 unnumbered interface 
```
sonic-cli(config)# interface Ethernet 0
sonic-cli(conf-if-Ethernet0)# ip unnumbered Loopback1
```
## ip unnumbered 
### Description 
```
Configure IPv4 unnumbered interface by borrowing IPv4 address from the Donor interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
ip unnumbered <donor-interface>
no ip unnumbered
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| donor-interface | String  | String  |
### Usage Guidelines 
```
Use this command to configure IPv4 unnumbered interface at the interface level.
```
### Examples 
#### Configure IPv4 unnumbered interface 
```
sonic-cli(config)# interface PortChannel 1
sonic-cli(conf-if-po1)# ip unnumbered Loopback1
```
## ip vrf 
### Description 
```
VRF instance configuration 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ip vrf <vrf-name>
no ip vrf <vrf-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |
## ip vrf forwarding 
### Description 
```
Configure forwarding table 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
ip vrf forwarding <vrf-name>
no ip vrf forwarding <vrf-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |
## ip vrf forwarding 
### Description 
```
Configure forwarding table 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
ip vrf forwarding <vrf-name>
no ip vrf forwarding <vrf-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |
## ip vrf forwarding 
### Description 
```
Configure forwarding table 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ip vrf forwarding <vrf-name>
no ip vrf forwarding <vrf-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |
## ip vrf forwarding 
### Description 
```
Configure forwarding table 
```
### Parent Commands (Modes) 
```
interface Loopback <lo-id>
```
### Syntax 
```
ip vrf forwarding <vrf-name>
no ip vrf forwarding <vrf-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |
## ip vrf management 
### Description 
```
Management VRF configuration 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ip vrf management
no ip vrf management
```
## ipv6 
### Description 
```
ipv6 prefix-list 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ipv6
no ipv6
```
## ipv6 address 
### Description 
```
IPv6 address 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
ipv6 address <addr>
no ipv6 address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A::B/mask  | String  |
## ipv6 address 
### Description 
```
IPv6 address 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
ipv6 address <addr> [ gwaddr ] <gw_addr>
no ipv6 address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A::B/mask  | String  |
| gw_addr | A::B  | String  |
## ipv6 address 
### Description 
```
IPv6 address 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
ipv6 address <addr>
no ipv6 address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A::B/mask  | String  |
## ipv6 address 
### Description 
```
IPv6 address 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ipv6 address <addr>
no ipv6 address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A::B/mask  | String  |
## ipv6 address 
### Description 
```
IPv6 address 
```
### Parent Commands (Modes) 
```
interface Loopback <lo-id>
```
### Syntax 
```
ipv6 address <addr>
no ipv6 address <addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A::B/mask  | String  |
## ipv6 anycast-address 
### Description 
```
Configures IPv6 Static Anycast Gateway Address for an Interface.
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
ipv6 anycast-address <anycast-addr>
no ipv6 anycast-address <anycast-addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| anycast-addr | A::B/mask  | String  |
## ipv6 anycast-address 

### Description 

```
Enable/Disable IPv4 Static Anycast Gateway functionality. By default it is enabled.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ipv6 anycast-address { enable | disable }

```
## ipv6 prefix-list 
### Description 
```
Build a prefix list 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ipv6 prefix-list <prefix-name> { { permit { <ipv6-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } | { deny { <ipv6-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } }
no ipv6 prefix-list <prefix-name> { { [ permit ] { <ipv6-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } | { [ deny ] { <ipv6-prefix> { [ ge ] <ge-min-prefix-length> } { [ le ] <le-max-prefix-length> } } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix-name | String  | String  |
| ipv6-prefix | A::B/mask  | String  |
| ge-min-prefix-length |   | Integer  |
| le-max-prefix-length |   | Integer  |
## kdump enable 

### Description 

```
Enable or disable KDUMP operation. These commands require a reboot to complete.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
kdump enable

```
### Usage Guidelines 

```
Use the command "kdump enable" to enable the kdump operation.
Use the command "no kdump" to disable the kdump operation.


```
### Examples 

```
sonic# configure terminal
sonic(config)# enable kdump
KDUMP configuration has been updated in the startup configuration
Kdump configuration changes will be applied after the system reboots
sonic(config)# no kdump
KDUMP configuration has been updated in the startup configuration
ALERT! A system reboot is highly recommended.
Kdump configuration changes will be applied after the system reboots


```
## kdump memory 
### Description 
```
Set or reset to default the amount of memory reserved for kdump.
These commands require a reboot to complete.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
kdump memory <kdump_memory>
no kdump memory
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| kdump_memory | Memory reserved for kdump  | String  |
### Usage Guidelines 
```
Use the commands "kdump memory <X>" or "no kdump memory" to set or reset to default the amount of memory reserved for kdump.
```
### Examples 
```
sonic# configure terminal
sonic(config)# kdump memory 512M
KDUMP configuration has been updated in the startup configuration
kdump updated memory will be only operational after the system reboots
sonic(config)# no kdump memory
```
## kdump num_dumps 
### Description 
```
Set or reset to default value the maximum number of kernel core files stored locally.
These commands typically require a reboot to complete.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
kdump num_dumps <kdump_num_dumps>
no kdump num_dumps
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| kdump_num_dumps | Maximum number of kernel core files stored locally  | Integer  |
### Usage Guidelines 
```
Use the commands "kdump num_dump <X>" or "no kdump num_dumps" to set or reset to default the maximum number of kernel core files stored locally.
```
### Examples 
```
sonic# configure terminal
sonic(config)# kdump num_dump 5
sonic(config)# no kdump num_dump 5
```
## keepalive-interval 

### Description 

```
Set mclag Session Keepalive interaval in secs 


```
### Parent Commands (Modes) 

```
mclag domain <mclag-domain-id>

```
### Syntax 

```
keepalive-interval <KA>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| KA | Keepalive Interval  | Integer  |


## link state track 
### Description 
```
Create link state tracking group 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
link state track <grp-name>
no link state track <grp-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-name | String(Max: 63 characters)  | String  |
## link state track 
### Description 
```
Link state tracking 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
link state track <grp-name> upstream
no link state track <grp-name> upstream
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-name | String(Max: 63 characters)  | String  |
## link state track 
### Description 
```
Link state tracking 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
link state track <grp-name> upstream
no link state track <grp-name> upstream
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-name | String(Max: 63 characters)  | String  |
## link state track 
### Description 
```
Link state tracking 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
link state track <grp-name> upstream
no link state track <grp-name> upstream
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-name | String(Max: 63 characters)  | String  |
## listen 
### Description 
```
This command create a listen range for BGP for dynamic BGP neighbors.
BGP will accept connections from any peers in the specified prefix. Configuration
from the specified peer-group is used to configure these peers.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
listen { { range { <addr> { peer-group <pgname> } } } | { limit <lmt-val> } }
no listen { { range { <addr> { [ peer-group ] <pgname> } } } | { limit <lmt-val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| addr | A.B.C.D/mask or A::B/mask  | String  |
| pgname | String  | String  |
| lmt-val |   | Integer  |
### Usage Guidelines 
```
Use this command to accept peering connection from neighbors and create
dynamic neighbors
```
### Examples 
#### Below command creates a listen range 192.168.0.0/16 
```
         sonic# configure terminal
         sonic(config)# router bgp 65300
         sonic(config-router-bgp)# listen range 192.168.0.0/16 peer-group PG_Ext
```
## local-as 
### Description 
```
This command specifies an alternate AS for this BGP process when
interacting with the specified peer. With no modifiers, the specified
local-as is prepended to the received AS_PATH when receiving routing
updates from the peer, and prepended to the outgoing AS_PATH (after the
process local AS) when transmitting local routes to the peer.
If the no-prepend CLI option is specified, then the supplied local-as is
not prepended to the received AS_PATH.
If the replace-as CLI option is specified, then only the supplied
local-as is prepended to the AS_PATH when transmitting local-route
updates to this peer.
Note that replace-as can only be specified if no-prepend is.
This command is only allowed for eBGP peers.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
local-as <asnum> { [ no-prepend ] [ replace-as ] }
no local-as
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| asnum | 1-4294967295  | Integer  |
### Usage Guidelines 
```
Use this command to configure local AS number for a BGP neighbor and
control how the local AS number is prepended to the AS_PATH of incoming
and outgoing routes.
```
### Examples 
#### Following command configures local as and enables          no-prepend for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# local-as 65200 no-prepend
```
## local-as 
### Description 
```
This command specifies an alternate AS for this BGP process when
interacting with the specified peers in a peer-group. With no modifiers, the specified
local-as is prepended to the received AS_PATH when receiving routing
updates from the peer, and prepended to the outgoing AS_PATH (after the
process local AS) when transmitting local routes to the peer.
If the no-prepend CLI option is specified, then the supplied local-as is
not prepended to the received AS_PATH.
If the replace-as CLI option is specified, then only the supplied
local-as is prepended to the AS_PATH when transmitting local-route
updates to this peer.
Note that replace-as can only be specified if no-prepend is.
This command is only allowed for eBGP peers.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
local-as <asnum> { [ no-prepend ] [ replace-as ] }
no local-as
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| asnum | 1-4294967295  | Integer  |
### Usage Guidelines 
```
Use this command to configure local AS number for BGP neighbors in a
peer-group and control how the local AS number is prepended to the
AS_PATH of incoming and outgoing routes.
```
### Examples 
#### Following command configures local AS and enables          no-prepend for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# local-as 65200 non-prepend
```
## log-neighbor-changes 
### Description 
```
This command enables logging of neighbor's state transition events
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
log-neighbor-changes
no log-neighbor-changes
```
### Usage Guidelines 
```
Use this command to enable logging of neighbor UP/Down events along with
reason code for down event.
```
### Examples 
#### Below command enables logging of BGP neighbor's up/down          events 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# log-neighbor-changes
```
## map 
### Description 
```
Command to configure VNI-VLAN mappings and VNI-VRF mappings
```
### Parent Commands (Modes) 
```
interface Vxlan <vxlan-if-name>
```
### Syntax 
```
map vni { <vnid> { { vlan { <vid> { [ count ] [ <numvid> ] } } } | { vrf <vrf-name> } } }
no map vni { <vnid> { { vlan <vid> { [ count ] [ <numvid> ] } } | { vrf <vrf-name> } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vnid |   | Integer  |
| vid |   | Integer  |
| numvid |   | Integer  |
| vrf-name | String(Max: 63 characters)  | String  |
### Usage Guidelines 
```
(conf-if-Vxlan-vtep)# map vni VNIID vlan VLANID count COUNT
(conf-if-Vxlan-vtep)# map vni VNIID vrf VRFNAME
VNIID - VNI value between 1 to 16777215
VLANID - VLAN value between 1 to 4094
COUNT - number of mappings (optional parameter)
VRFNAME - string
```
### Examples 
#### configure vni-vlan and vni-vrf mappings 
```
sonic(config)# interface Vxlan vtep1
sonic(conf-if-Vxlan-vtep1)# map vni 100 vlan 100 count 2
sonic(conf-if-Vxlan-vtep1)# map vni 100 vrf vrf1
```
## match as-path 
### Description 
```
Set routing policy match criteria as-path 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match as-path <as-path-name>
no match as-path
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-path-name | String  | String  |
## match community 
### Description 
```
Set routing policy match criteria to BGP community 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match community <community-name>
no match community
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| community-name | String  | String  |
## match ext-community 
### Description 
```
Set routing policy match criteria to BGP external community 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match ext-community <community-name>
no match ext-community
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| community-name | String  | String  |
## match interface 
### Description 
```
Set routing policy match criteria to interface 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match interface { { Ethernet <phy-if-name> } | { PortChannel <lag-id> } | { Vlan <vlan-id> } }
no match interface
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-name | Unsigned integer  | String  |
| lag-id |   | Integer  |
| vlan-id |   | Integer  |
## match ip address prefix-list 
### Description 
```
Set routing policy match criteria to ipv4 prefix-list 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match ip address prefix-list <prefix-list-name>
no match ip address prefix-list
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix-list-name | String  | String  |
## match ip next-hop prefix-list 
### Description 
```
Set routing policy match criteria to next-hop prefix-list 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match ip next-hop prefix-list <match-hop>
no match ip next-hop prefix-list
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-hop | String  | String  |
## match ipv6 address prefix-list 
### Description 
```
Set routing policy match criteria to ipv6 prefix-list 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match ipv6 address prefix-list <prefix-list-name>
no match ipv6 address prefix-list
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix-list-name | String  | String  |
## match local-preference 
### Description 
```
Set routing policy match criteria to local-preference 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match local-preference <match-loc>
no match local-preference
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-loc | Unsigned integer  | String  |
## match metric 
### Description 
```
Set routing policy match criteria to metric 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match metric <match-met>
no match metric
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-met | Unsigned integer  | String  |
## match origin 
### Description 
```
Specify BGP origin 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match origin { egp | igp | incomplete }
no match origin
```
## match peer 
### Description 
```
Set routing policy match criteria to peer ip 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match peer { <match-peer> | { Ethernet <phy-if-name> } | { PortChannel <lag-id> } | { Vlan <vlan-id> } }
no match peer
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-peer | A.B.C.D/A::B  | String  |
| phy-if-name | Unsigned integer  | String  |
| lag-id |   | Integer  |
| vlan-id |   | Integer  |
## match source-protocol 
### Description 
```
Specify source protocol 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match source-protocol { bgp | ospf | ospf3 | static | connected }
no match source-protocol
```
## match tag 
### Description 
```
redistributes routes in the routing table that match the specified tags. 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
match tag <match-tag>
no match tag
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| match-tag | 1-4294967295  | Integer  |
## max-med 
### Description 
```
This command instructs BGP to advertise routes with max MED value under
a given condition
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
max-med { { on-startup <stime> } | administrative } [ <maxmedval> ]
no max-med { { on-startup <stime> } | administrative } [ <maxmedval> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| stime |   | Integer  |
| maxmedval |   | Integer  |
### Usage Guidelines 
```
Use this command to instruct BGP to advertise routes with max MED value.
The command allows user to set the condition under which routes with max
MED value will be sent. One is during the startup for a prespecified
number of seconds. The other is permanently. User can also specify the
value for max MED.
```
### Examples 
#### Below command instructs BGP to send Max MED after          startup for 300seconds. Max MED value is set to 2000 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# max-med on-startup 300 2000
```
## maximum-paths 
### Description 
```
Sets the maximum number of equal cost multipath for eBGP.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
maximum-paths <paths>
no maximum-paths
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| paths |   | Integer  |
### Usage Guidelines 
```
Use this command to configure BGP to control the maximum number of equal cost
multipath routes to eBGP destinations. This command is per
address-family
```
### Examples 
#### Configures maximum equal cost multipath to 32 for eBGP 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# maximum-paths 32
```
## maximum-paths 
### Description 
```
Forward packets over multiple paths 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
maximum-paths <paths>
no maximum-paths
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| paths |   | Integer  |
## maximum-paths ibgp 
### Description 
```
Sets the maximum number of equal cost multipath for iBGP.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
maximum-paths ibgp <ipaths> [ equal-cluster-length ]
no maximum-paths ibgp
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ipaths |   | Integer  |
### Usage Guidelines 
```
Use this command to configure BGP to control the maximum number of equal cost
multipath routes to iBGP destinations. This command is per
address-family
```
### Examples 
#### Configures maximum equal cost multipath to 32 for iBGP 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# maximum-paths ibgp 32
```
## maximum-paths ibgp 
### Description 
```
iBGP-multipath 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
maximum-paths ibgp <ipaths> [ equal-cluster-length ]
no maximum-paths ibgp
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ipaths |   | Integer  |
## maximum-prefix 
### Description 
```
This command configures the maximum number of prefix to accept from this
BGP neighbor.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
### Usage Guidelines 
```
Use this command to set the upper limit on number of BGP prefixes to
accept from this neighbor. This command has optional parameters for
warning user when a threshold is reached and rsetarting BGP neighborship
when maximum prefix limit has exceeded.
```
### Examples 
#### Following command configures maximum prefix of 2000 from          neighbor 20.20.20.2. The command also configures a threhold of 80% and          the action to take is warning when the number of prefxies received          exceeds the max limit of 2000 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# maximum-prefix 2000 80 warning-only
```
## maximum-prefix 
### Description 
```
This command configures the maximum number of prefix to accept from
BGP neighbors in a peer-group.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
### Usage Guidelines 
```
Use this command to set the upper limit on number of BGP prefixes to
accept from neighbors in a peer-group. This command has optional parameters for
warning user when a threshold is reached and rsetarting BGP neighborship
when maximum prefix limit has exceeded.
```
### Examples 
#### Following command configures maximum prefix of 2000 from          neighbors in peer-group PG_Int. The command also configures a threhold of 80% and          the action to take is warning when the number of prefxies received          exceeds the max limit of 2000 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# maximum-prefix 2000 80 warning-only
```
## maximum-prefix 
### Description 
```
Maximum number of prefixes to accept from this peer 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
## maximum-prefix 
### Description 
```
Maximum number of prefixes to accept from this peer 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
## maximum-prefix 
### Description 
```
Maximum number of prefixes to accept from this peer 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
## maximum-prefix 
### Description 
```
Maximum number of prefixes to accept from this peer 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
maximum-prefix <max-prefix-val> { [ <threshold-val> ] { [ warning-only ] | { [ restart ] <interval> } } }
no maximum-prefix [ <max-prefix-val> ] { [ threshold-val ] | [ warning-only ] | { [ restart ] <val> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| max-prefix-val | 1-4294967295  | Integer  |
| threshold-val |   | Integer  |
| interval |   | Integer  |
## mclag 
### Description 
```
Configure MCLAG interface 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
mclag <domain_id>
no mclag <domain_id>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| domain_id |   | Integer  |
## mclag domain 
### Description 
```
Enter MCLAG Domain configuration mode 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
mclag domain <mclag-domain-id>
no mclag domain <mclag-domain-id>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| mclag-domain-id |   | Integer  |
## mclag-seperate-ip 
### Description 
```
Configure seperate IP on Vlan interface for L3 protocol support over MCLAG 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
mclag-seperate-ip
no mclag-seperate-ip
```
## mirror-session 
### Description 
```
Mirror session configuration 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
mirror-session <session-name>
no mirror-session <session-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| session-name | String  | String  |
## mtu 
### Description 
```
Configure MTU 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
mtu <mtu>
no mtu
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| mtu |   | Integer  |
## mtu 
### Description 
```
Configure MTU 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
mtu <mtu>
no mtu
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| mtu |   | Integer  |
## mtu 
### Description 
```
Configure MTU 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
mtu <mtu>
no mtu
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| mtu |   | Integer  |
## mtu 
### Description 
```
Configure MTU 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
mtu <mtu>
no mtu
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| mtu |   | Integer  |
## nat 

### Description 

```
NAT configuration 


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
nat

```
## nat-zone 
### Description 
```
NAT Zone 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
nat-zone <zone>
no nat-zone
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| zone |   | Integer  |
## nat-zone 
### Description 
```
NAT Zone 
```
### Parent Commands (Modes) 
```
interface Loopback <lo-id>
```
### Syntax 
```
nat-zone <zone>
no nat-zone
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| zone |   | Integer  |
## nat-zone 
### Description 
```
NAT Zone 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
nat-zone <zone>
no nat-zone
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| zone |   | Integer  |
## nat-zone 
### Description 
```
NAT Zone 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
nat-zone <zone>
no nat-zone
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| zone |   | Integer  |
## neigh_suppress 
### Description 
```
Enable ARP and ND Suppression 
```
### Parent Commands (Modes) 
```
interface <vlan-if-name>
```
### Syntax 
```
neigh_suppress
no neigh_suppress
```
## neighbor 
### Description 
```
This command creates a BGP neighbor
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
no neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip | A.B.C.D/A::B  | String  |
### Usage Guidelines 
```
Use this command to create a BGP neighbor. User can input neighbor's
IPv4/IPv6 address directly or can input an interface name for unnumbered
BGP neighbor.
```
### Examples 
#### Below command creates a BGP neighbor 30.30.30.3 
```
         sonic# configure terminal
         sonic(config)# router bgp 65300
         sonic(config-router-bgp)# neighbor 30.30.30.3
         sonic(config-router-bgp-neighbor)#
```
## network 
### Description 
```
This command enables user to add a network to announce via BGP
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
network <prefix> { [ backdoor ] { [ route-map ] <route-map-name> } }
no network <prefix> { [ backdoor ] { [ route-map ] <route-map-name> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix | A.B.C.D/mask  | String  |
| route-map-name | String  | String  |
### Usage Guidelines 
```
This command can be used by users and network administrators to
statically inject routes into BGP. User can use route-map optional
parameter to modify/set the various attributes of the route.
```
### Examples 
#### Creates a network 10.10.0.0/16 which will be announced            to all BGP neighbors 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# network 10.10.0.0/16
```
## network 
### Description 
```
Enable routing on an IP network 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
network <prefix> { [ backdoor ] { [ route-map ] <route-map-name> } }
no network <prefix> { [ backdoor ] { [ route-map ] <route-map-name> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| prefix | A::B/mask  | String  |
| route-map-name | String  | String  |
## network import-check 
### Description 
```
This command instructs BGP to check if BGP network route exists in local
route table before advertising the network
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
network import-check
no network import-check
```
### Usage Guidelines 
```
By default, BGP networks are adverised to neighbors irrespective of
whether the same route exists in local route table or not. This behavior
may lead to data traffic blackholing. User can use this command to put a
restriction on BGP networks to get advertised only if a corresponding
route from IGP exists in local route table.
```
### Examples 
#### Below command enables checking of presence of network in          local routing table before adverizing the network to neighbors 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# network import-check
```
## next-hop-self 
### Description 
```
This command sets next-hop attribute as it's own address in the outbound
route updates to this BGP neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
### Usage Guidelines 
```
Use this command to disable BGP next-hop attribute computation and
override the next-hop by sender's own address.
```
### Examples 
#### Following command configures next-hop-self for BGP          updates sent to neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# next-hop-self
```
## next-hop-self 
### Description 
```
This command sets next-hop attribute as it's own address in the outbound
route updates to BGP neighbors in a peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
### Usage Guidelines 
```
Use this command to disable BGP next-hop attribute computation and
override the next-hop by sender's own address.
```
### Examples 
#### Following command configures next-hop-self for BGP          updates sent to neighbors in peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# next-hop-self
```
## next-hop-self 
### Description 
```
Disable the next hop calculation for this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
## next-hop-self 
### Description 
```
Disable the next hop calculation for this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
## next-hop-self 
### Description 
```
Disable the next hop calculation for this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
## next-hop-self 
### Description 
```
Disable the next hop calculation for this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
next-hop-self [ force ]
no next-hop-self [ force ]
```
## override-capability 
### Description 
```
This command instructs BGP to override the result of Capability
Negotiation with local configuration. Ignore remote peer's capability
value.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
override-capability
no override-capability
```
### Usage Guidelines 
```
Use this command to ignored the negotiated capability parameters with
neighbor and instead use the locally configured parameters.
```
### Examples 
#### Following command instructs BGP to ignore the negotiated          parameters and use the locally configured one for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# override-capability
```
## override-capability 
### Description 
```
This command instructs BGP to override the result of Capability
Negotiation with local configuration. Ignore remote peer's capability
value.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
override-capability
no override-capability
```
### Usage Guidelines 
```
Use this command to ignored the negotiated capability parameters with
neighbors in a peer-group and instead use the locally configured parameters.
```
### Examples 
#### Following command instructs BGP to ignore the negotiated          parameters and use the locally configured one for neighbors in          peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# override-capability
```
## passive 
### Description 
```
This command makes BGP neighbor passive. That is, this BGP neighbor will
not initiate a session. However, it will listen to any incoming BGP
session.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
passive
no passive
```
### Usage Guidelines 
```
Use this command to set a BGP neighbor as passive.
```
### Examples 
#### Following command makes BGP neighbor 30.30.30.3 as          passive one 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# passive
```
## passive 
### Description 
```
This command makes BGP neighbors in a peer-group passive. That is, BGP
neighbors will not initiate a session. However, it will listen to any incoming BGP
session.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
passive
no passive
```
### Usage Guidelines 
```
Use this command to set BGP neighbors in a peer-group as passive.
```
### Examples 
#### Following command makes BGP neighbors in peer-group          PG_Ext passive 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# passive
```
## password 
### Description 
```
This command sets a MD5 password to be used with the tcp socket that is
being used to connect to the remote peer.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
password <String> [ encrypted ]
no password
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| String | String  | String  |
### Usage Guidelines 
```
This command is for security purposes. When Password is configures for a
BGP neighbor, sender will include a 16-bytes MD5 digest in TCP header of
BGP message and the receiver should be able to validate the digest then
only accept the BGP message.
```
### Examples 
#### Following command configures password for BGP neighbor          30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# password jackandjillwentupthehill
```
## password 
### Description 
```
This command sets a MD5 password to be used with the tcp socket that is
being used to connect to the remote peers in a peer-group.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
password <String> [ encrypted ]
no password
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| String | String  | String  |
### Usage Guidelines 
```
This command is for security purposes. When Password is configures for
BGP neighbors in a peer-group, sender will include a 16-bytes MD5 digest in TCP header of
BGP message and the receiver should be able to validate the digest then
only accept the BGP message.
```
### Examples 
#### Following command configures password for BGP neighbors          in a peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# password ilovebeansbecausetheyaremean
```
## peer 
### Description 
```
Configure single-hop and multi-hop Bidirectional Forwarding detection(BFD) peer.
```
### Parent Commands (Modes) 
```
bfd
```
### Syntax 
```
peer { <peer_ipv4> | <peer_ipv6> } [ vrf ] <vrfname> [ multihop ] [ local-address ] { <local_ipv4> | <local_ipv6> } [ interface ] <interfacename>
no peer { <peer_ipv4> | <peer_ipv6> } [ vrf ] <vrfname> [ multihop ] [ local-address ] { <local_ipv4> | <local_ipv6> } [ interface ] <interfacename>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| peer_ipv4 | A.B.C.D  | String  |
| peer_ipv6 | A::B  | String  |
| vrfname | String  | String  |
| local_ipv4 | A.B.C.D  | String  |
| local_ipv6 | A::B  | String  |
| interfacename | String  | String  |
### Usage Guidelines 
```
For single-hop BFD peer interace must be configured and for multi-hop BFD peer local address must be configured.
```
### Examples 
#### Configure single-hop BFD peer with default vrf 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
```
#### Configure single-hop BFD peer with user vrf 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0 vrf Vrf1
```
#### Configure multi-hop BFD peer with default vrf 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.2 multihop local-address 192.168.0.3
```
#### Configure multi-hop BFD peer with user vrf 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.2 multihop local-address 192.168.0.3 vrf Vrf1
```
## peer-group 
### Description 
```
This command creates a BGP peer-group
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
peer-group <template-str>
no peer-group <template>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| template-str | String  | String  |
### Usage Guidelines 
```
Use this command to create a BGP peer-group.
```
### Examples 
#### Below command creates a BGP peer-group named PG_Ext 
```
         sonic# configure terminal
         sonic(config)# router bgp 65300
         sonic(config-router-bgp)# peer-group PG_Ext
         sonic(config-router-bgp-pg)#
```
## peer-group 
### Description 
```
This command assigns a BGP neighbor to a peer-group
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
peer-group <template-name>
no peer-group [ <template-name> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| template-name | String  | String  |
### Usage Guidelines 
```
Assigning a BGP neighbor to a peer-group will inherit parameters from
peer-group.
```
### Examples 
#### Following command assigns neighbor 30.30.30.3 to          peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# peer-group PG_Ext
```
## peer-ip 
### Description 
```
Set mclag Peer IPv4 address 
```
### Parent Commands (Modes) 
```
mclag domain <mclag-domain-id>
```
### Syntax 
```
peer-ip <PIP>
no peer-ip
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| PIP | A.B.C.D  | String  |
## peer-link 
### Description 
```
Set mclag Peer Interface 
```
### Parent Commands (Modes) 
```
mclag domain <mclag-domain-id>
```
### Syntax 
```
peer-link { { Ethernet <PLK> } | { PortChannel <PLK> } }
no peer-link
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| PLK | Unsigned integer  | String  |
## pool 
### Description 
```
Create NAT Pool 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
pool <pool-name> <global-ip-range> [ <global-port-range> ]
no pool <pool-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pool-name | String  | String  |
| global-ip-range | String  | String  |
| global-port-range | String  | String  |
## port 
### Description 
```
This command sets TCP port for a BGP neighbor.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
port <tcpport>
no port
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tcpport |   | Integer  |
### Usage Guidelines 
```
Use this command to set a specific port for BGP neighbor. This command
is optional.
```
### Examples 
#### Following command configures TCP port for BGP neighbor          30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# port 61356
```
## port 
### Description 
```
This command sets TCP port for BGP neighbors in a peer-group.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
port <tcpport>
no port
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tcpport |   | Integer  |
### Usage Guidelines 
```
Use this command to set a specific port for BGP neighbors in a
peer-group. This command is optional.
```
### Examples 
#### Following command configures TCP port for BGP peer-group          PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# port 65001
```
## prefix-list 
### Description 
```
This command configures prefix list for a BGP neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
### Usage Guidelines 
```
Use this command to define policy (route filtering) for a BGP neighbor
in outbound or/and inbound direction.
```
### Examples 
#### Following command configures a prefix-list          pl_allow_remote in inbound direction for neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# prefix-list pl_allow_remote in
```
## prefix-list 
### Description 
```
This command configures prefix list for a BGP peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
### Usage Guidelines 
```
Use this command to define policy (route filtering) for a BGP peer-group
in outbound or/and inbound direction.
```
### Examples 
#### Following command configures a prefix-list          pl_allow_remote in inbound direction for peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# prefix-list pl_allow_remote in
```
## prefix-list 
### Description 
```
Filter updates to/from this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
## prefix-list 
### Description 
```
Filter updates to/from this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
## prefix-list 
### Description 
```
Filter updates to/from this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
## prefix-list 
### Description 
```
Filter updates to/from this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
prefix-list <pname> { in | out }
no prefix-list <pname> { in | out }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pname | String  | String  |
## ptp announce-timeout 

### Description 

```
Configure PTP announce receipt timeout value. The default value is 3.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp announce-timeout <ptp_announce_timeout>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_announce_timeout |   | Integer  |


### Examples 

```
sonic(config)# ptp announce-timeout 2
Success


```
## ptp domain 

### Description 

```
Configure PTP domain


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp domain <ptp_domain>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_domain |   | Integer  |


### Examples 

```
sonic(config)# ptp domain 1
Success


```
## ptp domain-profile 

### Description 

```
Configure PTP domain profile


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp domain-profile <ptp_domain_profile>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_domain_profile |   | Select [default(ieee1588) g8275.1(G.8275.1) g8275.2(G.8275.2) ]  |


### Examples 

```
sonic(config)# ptp domain-profile default
Success


```
## ptp ipv6-scope 

### Description 

```
Configure PTP IPv6 multicast address scope


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp ipv6-scope <ptp_ipv6_scope>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_ipv6_scope | Hexadecimal range (0x0-0xf)  | String  |


### Examples 

```
sonic(config)# ptp ipv6-scope 0xe
Success


```
## ptp log-announce-interval 

### Description 

```
Configure PTP log announce interval value. The interval should be the sam in the whole domain. It's specified as a power of two in seconds. The default is 1 (2 seconds).


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp log-announce-interval <ptp_announce_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_announce_interval |   | Integer  |


### Examples 

```
sonic(config)# ptp log-announce-interval 0
Success


```
## ptp log-min-delay-req-interval 

### Description 

```
Configure PTP log min delay req interval value. It is specified as a power of two in seconds. The default is 0 (1 second).


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp log-min-delay-req-interval <ptp_delay_request_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_delay_request_interval |   | Integer  |


### Examples 

```
sonic(config)# ptp log-min-delay-req-interval 0
Success


```
## ptp log-sync-interval 

### Description 

```
Configure PTP log sync interval value. It is specified as a power of two in seconds. The default is 0 (1 second).


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp log-sync-interval <ptp_sync_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_sync_interval |   | Integer  |


### Examples 

```
sonic(config)# ptp log-sync-interval 0
Success


```
## ptp mode 

### Description 

```
Configure PTP clock type


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp mode <mode_type>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mode_type | PTP mode  | Select [boundary-clock(BC) peer-to-peer-transparent-clock(P2P_TC) end-to-end-transparent-clock(E2E_TC) disable(disable) ]  |


### Examples 

```
sonic(config)# ptp mode boundary-clock
Success


```
## ptp network-transport 

### Description 

```
Configure PTP network-transport


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp network-transport <ptp_network_transport_type> <ptp_master_slave>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_network_transport_type |   | Select [l2(L2) ipv4(UDPv4) ipv6(UDPv6) ]  |
| ptp_master_slave | unicast/multicast  | Select [unicast(unicast) multicast(multicast) ]  |


### Examples 

```
sonic(config)# ptp network-transport ipv4 unicast
Success


```
## ptp port add 

### Description 

```
Add a PTP port


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp port add { Ethernet <ptp_port_number> }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_port_number | Unsigned integer  | String  |


### Examples 

```
sonic(config)# ptp port add Ethernet 64
Success


```
## ptp port del 

### Description 

```
Delete a PTP port


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp port del { Ethernet <ptp_port_number> }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_port_number | Unsigned integer  | String  |


### Examples 

```
sonic(config)# ptp port del Ethernet 64
Success


```
## ptp port master-table 

### Description 

```
Add/Delete a master IP/MAC from the master table for the designated slave port


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp port master-table { Ethernet <ptp_port_number> } { { add { <l3_ip> | <mac> } } | { del { <l3_ip> | <mac> } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_port_number | Unsigned integer  | String  |
| l3_ip | A.B.C.D/A::B  | String  |
| mac | nn:nn:nn:nn:nn:nn  | String  |


### Examples 

```
sonic(config)# ptp port master-table Ethernet 64 add 10.1.1.1
Success
sonic(config)# ptp port master-table Ethernet 64 del 10.1.1.1
Success


```
## ptp priority1 

### Description 

```
Configure PTP priority1 value


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp priority1 <ptp_priority1>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_priority1 |   | Integer  |


### Examples 

```
sonic(config)# ptp priority1 128
Success


```
## ptp priority2 

### Description 

```
Configure PTP priority2 value


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp priority2 <ptp_priority2>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_priority2 |   | Integer  |


### Examples 

```
sonic(config)# ptp priority2 128
Success


```
## ptp two-step 

### Description 

```
Configure PTP two-step mode


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
ptp two-step <ptp_two_step>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_two_step | enable or disable  | Select [enable(enable) disable(disable) ]  |


### Examples 

```
sonic(config)# ptp two-step enable
Success


```
## radius-server auth-type 
### Description 
```
Configure global authentication type for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server auth-type <auth_type>
no radius-server auth-type
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| auth_type | authentication type  | Select [pap(pap) chap(chap) mschapv2(mschapv2) ]  |
## radius-server host 
### Description 
```
Configure a server for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server host <host> [ auth-port ] <vauth_port> [ timeout ] <vtimeout> [ retransmit ] <vretransmit> [ key ] <vkey> [ auth-type ] <vauth_type> [ priority ] <vpriority> [ vrf ] <vvrf>
no radius-server host <host> { [ auth-port ] | [ timeout ] | [ retransmit ] | [ key ] | [ auth-type ] | [ priority ] | [ vrf ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| host | A.B.C.D/A::B  | String  |
| vauth_port | port  | Integer  |
| vtimeout | seconds  | Integer  |
| vretransmit | attempts  | Integer  |
| vkey | (Valid Chars: ASCII printable except SPACE, #, and COMMA, Max Len: 65) shared secret  | String  |
| vauth_type | authentication type  | Select [pap(pap) chap(chap) mschapv2(mschapv2) ]  |
| vpriority | (1..64)  | Integer  |
| vvrf | Name of VRF (Max size 32, (mgmt, or prefixed by Vrf_)  | String  |
## radius-server key 
### Description 
```
Configure global shared secret for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server key <key>
no radius-server key
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| key | (Valid Chars: ASCII printable except SPACE, #, and COMMA, Max Len: 65) shared secret  | String  |
## radius-server retransmit 
### Description 
```
Configure global retransmit attempts for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server retransmit <retransmit>
no radius-server retransmit
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| retransmit | attempts  | Integer  |
## radius-server source-ip 
### Description 
```
Configure global source ip for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server source-ip <source_ip>
no radius-server source-ip
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| source_ip | A.B.C.D/A::B  | String  |
## radius-server timeout 
### Description 
```
Configure global timeout for RADIUS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
radius-server timeout <timeout>
no radius-server timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| timeout | seconds  | Integer  |
## rd 
### Description 
```
Route distinguisher 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
rd <rdvalue>
no rd <rdvalue>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rdvalue | String  | String  |
## rd 
### Description 
```
Route distinguisher 
```
### Parent Commands (Modes) 
```
vni <vninum>
```
### Syntax 
```
rd <rdvalue>
no rd <rdvalue>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rdvalue | String  | String  |
## read-quanta 
### Description 
```
This command configures the maximum number of BGP packets to read from
peer socker in one cycle of I/O
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
read-quanta <rdval>
no read-quanta
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rdval |   | Integer  |
### Usage Guidelines 
```
BGP packets are read off the wire one at a time in a loop. This setting
controls how many iterations the loop runs for. It is best to leave this
setting on the default.
```
### Examples 
#### Below command configures the read-quanta to          6 packets 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# read-quanta 6
```
## receive-interval 

### Description 

```
Configure packet receive interval for Bidirectional Forwarding detection(BFD) peer.


```
### Parent Commands (Modes) 

```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>

```
### Syntax 

```
receive-interval <receive_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| receive_interval |   | Integer  |


### Usage Guidelines 

```
This command can be used to configure desired packet receive interval from BFD peer, default value is 300 milliseconds.


```
### Examples 
#### Configure packet receive interval 

```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# receive-interval 200


```
## redistribute 
### Description 
```
Redistribute information from another routing protocol to BGP. User will
have an option to apply a route-map to control the routes that can be
redistributed into BGP.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
redistribute { connected | static | ospf } [ route-map ] <route-map-name> [ metric ] <metvalue>
no redistribute { connected | static | ospf } [ route-map ] <route-map-name> [ metric ] <metvalue>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-map-name | String  | String  |
| metvalue |   | Integer  |
### Usage Guidelines 
```
User can provide a route-map while enabling redistribution of routes to
control the routes that goes into BGP. User can also use metric option
to set the default metric for the redistributed routes.
```
### Examples 
#### Enable redistribution of connected routes into BGP 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# redistribute connected
```
## redistribute 
### Description 
```
Redistribute information from another routing protocol 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
redistribute { connected | static | ospfv3 } [ route-map ] <route-map-name> [ metric ] <metvalue>
no redistribute { connected | static | ospfv3 } [ route-map ] <route-map-name> [ metric ] <metvalue>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-map-name | String  | String  |
| metvalue |   | Integer  |
## remote-as 
### Description 
```
This command configure the remote-as number for a BGP neighbor. This
command also can tag a neighbor (dynmaic) as internal (iBGP) or external (eBGP)
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
remote-as { internal | external | <as-num-dot> }
no remote-as { [ internal ] | [ external ] | [ <as-num-dot> ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-num-dot | 1-4294967295  | Integer  |
### Usage Guidelines 
```
remote-as configuration for a BGP neighbor is mandatory. User must
configure remote-as right after creating the BGP neighbor. User can
either specify the remote AS number or can specify whether a neighbor is
internal or external.
```
### Examples 
#### Following command configures remote AS number for neighbor          30.30.30.3 to 65100 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# remote-as 65100
```
## remote-as 
### Description 
```
This command configure the remote-as number for a BGP peer-group. This
command also can tag a peer-group as internal (iBGP) or external (eBGP)
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
remote-as { internal | external | <as-num-dot> }
no remote-as { [ internal ] | [ external ] | [ <as-num-dot> ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-num-dot | 1-4294967295  | Integer  |
### Usage Guidelines 
```
This command configures remote-as number for a BGP peer-group.
User can either specify the remote AS number or can specify whether
a peer-group is internal or external.
```
### Examples 
#### Following command configures remote AS number for          peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# remote-as 65200
```
## remove-private-AS 
### Description 
```
This command configures BGP to remove private AS numbers from as-path in
outbound BGP updates to neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
### Usage Guidelines 
```
Use this command at the boundary of your BGP network to remove
the internal/private AS numbers from outbound route updates. User can
optionally choose to replace private AS number by local AS number.
```
### Examples 
#### Following command enables BGP to remove all private AS          numbers from outbound updates to neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# remove-private-AS all
```
## remove-private-AS 
### Description 
```
This command configures BGP to remove private AS numbers from as-path in
outbound BGP updates to neighbors in a peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
### Usage Guidelines 
```
Use this command at the boundary of your BGP network to remove
the internal/private AS numbers from outbound route updates. User can
optionally choose to replace private AS number by local AS number.
```
### Examples 
#### Following command enables BGP to remove all private AS          numbers from outbound updates to peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# remove-private-AS all
```
## remove-private-AS 
### Description 
```
Remove private ASNs in outbound updates 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
## remove-private-AS 
### Description 
```
Remove private ASNs in outbound updates 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
## remove-private-AS 
### Description 
```
Remove private ASNs in outbound updates 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
## remove-private-AS 
### Description 
```
Remove private ASNs in outbound updates 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
remove-private-AS [ all ] [ replace-AS ]
no remove-private-AS [ all ] [ replace-AS ]
```
## route-map 
### Description 
```
This command configures policy for BGP neighbor using a route-map. The
policy can be applied in INBOUND or OUTBOUND direction
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
### Usage Guidelines 
```
Use this command to configure policy for BGP neighbor. The policy can be
applied in inbound or outbound direction. The policy will dicatate if a
subset of routes needs to be filtered out or/and if attributes of some
routes needs to be modified
```
### Examples 
#### Following command configures a route-map for BGP          neighbor in inbound direction 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# route-map rmap_filter_intra_routes in
```
## route-map 
### Description 
```
This command configures policy for BGP neighbors in peer-group using a route-map. The
policy can be applied in INBOUND or OUTBOUND direction
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
### Usage Guidelines 
```
Use this command to configure policy for BGP peer-group. The policy can be
applied in inbound or outbound direction. The policy will dicatate if a
subset of routes needs to be filtered out or/and if attributes of some
routes needs to be modified
```
### Examples 
#### Following command configures a route-map for BGP          peer-group in inbound direction 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# route-map RM_Blk_192 in
```
## route-map 
### Description 
```
Name of the route map (max 140 chars) 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
## route-map 
### Description 
```
Name of the route map (max 140 chars) 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
## route-map 
### Description 
```
Name of the route map (max 140 chars) 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
## route-map 
### Description 
```
Name of the route map (max 140 chars) 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-map <route-name-str> { in | out }
no route-map <route-name-str> { [ in ] | [ out ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-name-str | String  | String  |
## route-map 
### Description 
```
Specify routing policy 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
route-map <route-map-name> { permit | deny } <seq-nu>
no route-map <route-map-name> { { [ permit ] <seq-nu> } | { [ deny ] <seq-nu> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| route-map-name | String(Max: 63 characters)  | String  |
| seq-nu |   | Integer  |
## route-map delay-timer 
### Description 
```
This command sets the route-map change processing delay interval in
seconds.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
route-map delay-timer <delaytm>
no route-map delay-timer
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| delaytm |   | Integer  |
### Usage Guidelines 
```
Change in route-map may require BGP RIB to get re-processed to reflect
the change in policy. This command set the interval in seconds to wait before processing
route-map change.
```
### Examples 
#### Below command set the route-map change delay to          60seconds 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# route-map delay-timer 60
```
## route-reflector allow-outbound-policy 
### Description 
```
This command allows to set the outbound policy for route reflector
neighbors.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
route-reflector allow-outbound-policy
no route-reflector allow-outbound-policy
```
### Usage Guidelines 
```
Use this command to allow users to set outbound policy for route
reflector neighbors.
```
### Examples 
#### Below command enables route-policy for route reflector          BGP neighbors 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# route-reflector allow-outbound-policy
```
## route-reflector-client 
### Description 
```
This command configures a BGP neighbor as route reflector client.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
### Usage Guidelines 
```
Use this command to configure an IBGP neighbor a route reflector client.
This command will implicitly make the local router a route reflector
server.
```
### Examples 
#### Following command configures neighbor 20.20.20.2 as          route reflector client 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# route-reflector-client
```
## route-reflector-client 
### Description 
```
This command configures BGP neighbors in a peer-group as route reflector client.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
### Usage Guidelines 
```
Use this command to configure an IBGP peer-group route reflector client.
```
### Examples 
#### Following command configures neighbors in a peer-group as          route reflector client 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# route-reflector-client
```
## route-reflector-client 
### Description 
```
Configure a neighbor as Route Reflector client 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
## route-reflector-client 
### Description 
```
Configure a neighbor as Route Reflector client 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
## route-reflector-client 
### Description 
```
Configure a neighbor as Route Reflector client 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
## route-reflector-client 
### Description 
```
Configure a neighbor as Route Reflector client 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-reflector-client
no route-reflector-client
```
## route-server-client 
### Description 
```
This command configures a BGP neighbor a route server client.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-server-client
no route-server-client
```
### Usage Guidelines 
```
Use this command to configure an IBGP neighbor a route server client.
```
### Examples 
#### Following command configures neighbor 20.20.20.2 as          route server client 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# route-server-client
```
## route-server-client 
### Description 
```
This command configures BGP neighbors in a peer-group route server client.
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
route-server-client
no route-server-client
```
### Usage Guidelines 
```
Use this command to configure an IBGP peer-group route server client.
```
### Examples 
#### Following command configures neighbors in a peer-group as          route server client 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# route-server-client
```
## route-server-client 
### Description 
```
Configure a neighbor as Route Server client 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-server-client
no route-server-client
```
## route-server-client 
### Description 
```
Configure a neighbor as Route Server client 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
route-server-client
no route-server-client
```
## route-server-client 
### Description 
```
Configure a neighbor as Route Server client 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-server-client
no route-server-client
```
## route-server-client 
### Description 
```
Configure a neighbor as Route Server client 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-server-client
no route-server-client
```
## route-target 
### Description 
```
Route target 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
route-target <rttype> <rt>
no route-target <rttype> <rt>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rttype | Advertise options both or import or export  | Select [both(both) import(import) export(export) ]  |
| rt | String  | String  |
## route-target 
### Description 
```
Route target 
```
### Parent Commands (Modes) 
```
vni <vninum>
```
### Syntax 
```
route-target <rttype> <rt>
no route-target <rttype> <rt>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rttype | Advertise options both or import or export  | Select [both(both) import(import) export(export) ]  |
| rt | String  | String  |
## router 
### Description 
```
This command creates an instnace of BGP routing protocol in a VRF.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
no router bgp { [ vrf ] <vrf-name> }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-num-dot | 1-4294967295  | Integer  |
| vrf-name | String(Max: 15 characters)  | String  |
### Usage Guidelines 
```
Use this config to create BGP routing instance in a VRF. If vrf key is
not supplied by user, default-vrf is assumed. Only one instance of BGP
protocol can be created in a VRF. Attempt to create more than one
instance will result in command execution failure.
If a BGP instance already exists, executing this command with same AS
number will simply enter into the "router bgp ..." conifguration mode of
the CLI.
```
### Examples 
#### Below command creates a new BGP instance in default VRF          with local AS number as 65300 
```
sonic# configure terminal
sonic(config)# router bgp 65300
```
## router-id 
### Description 
```
This command configures router ID for an instance of BGP protocol
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
router-id <ip-addr>
no router-id
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A.B.C.D  | String  |
### Usage Guidelines 
```
Use this command to configure router ID for an instance of BGP protocol.
Router ID configuration is optional for user. BGP automatically picks up
one of the interface IP address as router ID if not configured
explicitly by user.
```
### Examples 
#### Below command configures router ID for BGP instance on          default-VRF 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# router-id 163.134.6.97
```
## router-id 

### Description 

```
This command configures router ID for an instance of BGP protocol


```
### Syntax 

```
router-id <ip-addr>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A.B.C.D  | String  |


### Usage Guidelines 

```
Use this command to configure router ID for an instance of BGP protocol.
Router ID configuration is optional for user. BGP automatically picks up
one of the interface IP address as router ID if not configured
explicitly by user.


```
### Examples 
#### Below command configures router ID for BGP instance on          default-VRF 

```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# router-id 163.134.6.97


```
## sample 
### Description 
```
This CLI is used to create a sample session that co-relates a sampling rate with a session name.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
sample <sample-name> rate <rate-name>
no sample <sample-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| sample-name | String(Max: 63 characters)  | String  |
| rate-name | Sampling rate  | Integer  |
### Usage Guidelines 
```
The sample session is identified by the name and can be used by multiple features to indicate sampling configuration. One packet in every rate packets will be sampled.
```
### Examples 
#### Configure Sample Session and sampling rate 
```
sonic(config)# sample s1 rate 5000
```
## send-community 
### Description 
```
This command configures BGP to send community to a neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
send-community { standard | extended | both | large | all | none }
no send-community
```
### Usage Guidelines 
```
Use this command to enable sending of community attribute to a BGP
neighbor. The command option provides the flexibility to enable sending
of standard, extended, large communities.
```
### Examples 
#### Following command enables BGP to send community          attribute to neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# send-community
```
## send-community 
### Description 
```
This command configures BGP to send community to neighbors in a
peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
send-community { standard | extended | both | large | all | none }
no send-community
```
### Usage Guidelines 
```
Use this command to enable sending of community attribute to BGP
neighbors in a peer-group. The command option provides the flexibility to enable sending
of standard, extended, large communities.
```
### Examples 
#### Following command enables BGP to send community          attribute to neighbors in a peer-group PG_Int 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# send-community
```
## send-community 
### Description 
```
Send Community attribute to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
send-community { standard | extended | both | large | all | none }
no send-community
```
## send-community 
### Description 
```
Send Community attribute to this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
send-community { standard | extended | both | large | all | none }
no send-community
```
## send-community 
### Description 
```
Send Community attribute to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
send-community { standard | extended | both | none }
no send-community
```
## send-community 
### Description 
```
Send Community attribute to this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
send-community { standard | extended | both | none }
no send-community
```
## seq 
### Description 
```
Sequence number 
```
### Parent Commands (Modes) 
```
ip access-list <access-list-name>
```
### Syntax 
```
seq <seq-no> { { deny { { <protocol> { <src-prefix> | src-any } { <dest-prefix> | dest-any } { [ dscp ] <dscp-val> } } | { icmp { <src-prefix> | src-any } { <dest-prefix> | dest-any } { [ dscp ] <dscp-val> } } | { tcp { <src-prefix> | src-any } { { [ src-eq ] <src-port-number> } } { <dest-prefix> | dest-any } { { [ dst-eq ] <dst-port-number> } } { [ dscp ] <dscp-val> } [ fin ] [ syn ] [ rst ] [ psh ] [ ack ] [ urg ] } | { udp { <src-prefix> | src-any } { { [ src-eq ] <src-port-number> } } { <dest-prefix> | dest-any } { { [ dst-eq ] <dst-port-number> } } { [ dscp ] <dscp-val> } } } } | { permit { { <proto-num> { <src-prefix> | src-any } { <dest-prefix> | dest-any } { [ dscp ] <dscp-val> } } | { icmp { <src-prefix> | src-any } { <dest-prefix> | dest-any } { [ dscp ] <dscp-val> } } | { tcp { <src-prefix> | src-any } { { [ src-eq ] <src-port-number> } } { <dest-prefix> | dest-any } { { [ dst-eq ] <dst-port-number> } } { [ dscp ] <dscp-val> } [ fin ] [ syn ] [ rst ] [ psh ] [ ack ] [ urg ] } | { udp { <src-prefix> | src-any } { { [ src-eq ] <src-port-number> } } { <dest-prefix> | dest-any } { { [ dst-eq ] <dst-port-number> } } { [ dscp ] <dscp-val> } } } } }
no seq <seq-no>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| seq-no |   | Integer  |
| protocol |   | Integer  |
| src-prefix | A.B.C.D/mask  | String  |
| dest-prefix | A.B.C.D/mask  | String  |
| dscp-val |   | Integer  |
| src-port-number |   | Integer  |
| dst-port-number |   | Integer  |
| proto-num |   | Integer  |
## session-timeout 
### Description 
```
Set mclag Session Timeout in secs 
```
### Parent Commands (Modes) 
```
mclag domain <mclag-domain-id>
```
### Syntax 
```
session-timeout <ST>
no session-timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ST |   | Integer  |
## set as-path 
### Description 
```
Transform BGP AS-path attribute 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set as-path { prepend { <as-number_list> } }
no set as-path prepend
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| as-number_list | asn list  | String  |
## set community 
### Description 
```
BGP community attribute 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set community { <comm-num> | local-AS | no-advertise | no-export | no-peer }
no set community { [ <comm-num> ] | [ local-AS ] | [ no-advertise ] | [ no-export ] | [ no-peer ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| comm-num | AA:NN  | String  |
## set extcommunity 
### Description 
```
BGP extended community attribute 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set extcommunity { { rt <value> } | { soo <value> } }
no set extcommunity { { [ rt ] <value> } | { [ soo ] <value> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value | ASN:NN_OR_IP-ADDRESS:NN  | String  |
## set ip 
### Description 
```
IP information 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set ip next-hop <ip-addr>
no set ip next-hop <ip-addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A.B.C.D  | String  |
## set local-preference 
### Description 
```
BGP local preference path attribute 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set local-preference <pvalue>
no set local-preference [ <pvalue> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| pvalue |   | Integer  |
## set metric 
### Description 
```
Metric value for destination routing protocol 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set metric <met>
no set metric [ <pvalue> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| met |   | Integer  |
## set origin 
### Description 
```
BGP origin code 
```
### Parent Commands (Modes) 
```
route-map <route-map-name> { permit | deny } <seq-nu>
```
### Syntax 
```
set origin { egp | igp | incomplete }
no set origin { [ egp ] | [ igp ] | [ incomplete ] }
```
## sflow agent-id 
### Description 
```
Configure sFlow agent interface
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
sflow agent-id <interface>
no sflow agent-id
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| interface |   |   |
### Examples 
```
sonic(config)# sflow agent-id Ethernet0
sonic(config)#
```
## sflow collector 
### Description 
```
Add an sFLow Collector
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
sflow collector <name> <ip> [ <port> ]
no sflow collector <name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 16 characters)  | String  |
| ip | A.B.C.D or A:B:C:D:E:F:G:H  | String  |
| port |   | Integer  |
### Examples 
#### Add an sFlow collector using default port 6343 
```
sonic(config)# sflow collector col1 1.1.1.1
sonic(config)#
```
#### Add an sFlow collector with port number 
```
sonic(config)# sflow collector col2 1.1.1.2 port 4451
sonic(config)#
```
## sflow enable 
### Description 
```
Enable sflow 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
sflow enable
no sflow enable
```
## sflow enable 
### Description 
```
Enable sFlow
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
sflow enable
no sflow enable
```
### Examples 
```
sonic(config)# sflow enable
sonic(config)#
```
## sflow polling-interval 
### Description 
```
Configure sFlow polling interval
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
sflow polling-interval <interval>
no sflow polling-interval
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| interval | 0 to disable  | Integer  |
### Examples 
```
sonic(config)# sflow polling-interval 44
sonic(config)#
```
## sflow sampling-rate 
### Description 
```
Set sampling-rate 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
sflow sampling-rate <rate>
no sflow sampling-rate
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rate |   | Integer  |
## show NeighbourSuppressStatus 

### Description 

```
Show arp and nd suppression status 


```
### Syntax 

```
show NeighbourSuppressStatus [ <id> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| id |   | Integer  |


## show PortChannel summary 

### Description 

```
LAG status and configurationn 


```
### Syntax 

```
show PortChannel summary

```
## show Vlan 

### Description 

```
Show Vlan commands 


```
### Syntax 

```
show Vlan [ <id> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| id |   | Integer  |


## show aaa 

### Description 

```
Show aaa info 


```
### Syntax 

```
show aaa

```
## show bfd peer 

### Description 

```
Display specific Bidirectional Forwarding detection(BFD) peer with the specificed filters..


```
### Syntax 

```
show bfd peer { <peer_ipv4> | <peer_ipv6> } [ vrf ] <vrfname> [ multihop ] [ local-address ] { <local_ipv4> | <local_ipv6> } [ interface ] <interfacename>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| peer_ipv4 | A.B.C.D  | String  |
| peer_ipv6 | A::B  | String  |
| vrfname | String  | String  |
| local_ipv4 | A.B.C.D  | String  |
| local_ipv6 | A::B  | String  |
| interfacename | String  | String  |


### Examples 
#### Display singlehop peer 

```
device# show bfd peer 192.168.2.1 interface Ethernet0


```
#### Display multihop peer 

```
device# show bfd peer 192.168.2.1 mulithop local-address 192.168.2.2


```
## show bfd peer counters 

### Description 

```
Displays counters for the specified Bidirectional Forwarding detection(BFD) peer with the input filters.


```
### Syntax 

```
show bfd peer counters { <peer_ipv4> | <peer_ipv6> } [ vrf ] <vrfname> [ multihop ] [ local-address ] { <local_ipv4> | <loacl_ipv6> } [ interface ] <interfacename>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| peer_ipv4 | A.B.C.D  | String  |
| peer_ipv6 | A::B  | String  |
| vrfname | String  | String  |
| local_ipv4 | A.B.C.D  | String  |
| loacl_ipv6 | A::B  | String  |
| interfacename | String  | String  |


### Examples 
#### Display singlehop peer counters 

```
device# show bfd peer counters 192.168.2.1 interface Ethernet0


```
#### Display multihop peer 

```
device# show bfd peer counters 192.168.2.1 mulithop local-address 192.168.2.2


```
## show bfd peers 

### Description 

```
Displays all Bidirectional Forwarding detection(BFD) peers.


```
### Syntax 

```
show bfd peers [ vrf ] <vrfname> [ brief ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrfname | String  | String  |


### Examples 
#### Display BFD peers 

```
device# show bfd peers


```
## show bfd peers counters 

### Description 

```
Displays counters for all the Bidirectional Forwarding detection(BFD) peers.


```
### Syntax 

```
show bfd peers counters

```
### Examples 
#### Display BFD peers 

```
device# show bfd peers counters


```
## show bgp as-path-access-list 

### Description 

```
This command displays BGP AS Path lists configured on the device.


```
### Syntax 

```
show bgp as-path-access-list [ <list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| list-name | String  | String  |


### Usage Guidelines 

```
User configures AS Path lists to use it in route-maps and with
neighbors to design BGP routing policies. This command enables users
to display the AS Path lists configured on this device. User can
provide AS path list name optional CLI key to display only that AS
Path list. If AS Path list name is not specified, all AS Path lists will
be displayed by this command.


```
### Examples 
#### The following command displays all AS Path lists            configured in BGP 

```
sonic# show bgp as-path-access-list
AS path list asp_private:
   members: ^65000.*6510565109$,65107.*65200
AS path list asp_public:
   members: ^107.*2301.*709$,97.*201


```
## show bgp community-list 

### Description 

```
This command displays BGP community lists configured on the device.


```
### Syntax 

```
show bgp community-list [ <list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| list-name | String  | String  |


### Usage Guidelines 

```
User configures community-list to use it in route-maps to design BGP
routing policies. This command enables users to display the community
lists configured on this device. User can provide community list name
optional CLI key to display only that community list. If community list
name is not specified, all community lists will be displayed by this command.


```
### Examples 
#### The following command displays all communities            configured in BGP 

```
sonic# show bgp community-list
Expanded community list CommList_Exp:   match: ANY
     300:500
     800:900
     no-export
Standard community list CommList_RT:  match: ANY
     100:200
     no-export
     no-peer
     65100:3456


```
## show bgp ext-community-list 

### Description 

```
This command displays BGP extended community lists configured on the device.


```
### Syntax 

```
show bgp ext-community-list [ <list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| list-name | String  | String  |


### Usage Guidelines 

```
User configures extended community-list to use it in route-maps to design BGP
routing policies. This command enables users to display the extended community
lists configured on this device. User can provide extended community list name
optional CLI key to display only that extended community list. If
extended community list name is not specified, all extended community lists will
be displayed by this command.


```
### Examples 
#### The following command displays all extended communities            configured in BGP 

```
sonic# show bgp ext-community-list
Standard extended community list ExtComm_AllowInt:  match: ALL
     rt:19.32.56.167:65011,rt:31.67.182.214:3001,soo:01:65010,soo:.13.175.21:65101
Standard extended community list ExtComm_BlockExt:  match: ANY
     rt:4020:65104
     soo:9.54.32.165:65200


```
## show bgp l2vpn evpn route 

### Description 

```
EVPN Route information 


```
### Syntax 

```
show bgp l2vpn evpn route { [ rd ] { <rdvalue> { { [ mac ] { <macvalue> { ip <ipvalue> } } } | { [ type ] { ead | es | macip | multicast | prefix } } } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| rdvalue | A.B.C.D:NN or ASN:NN  | String  |
| macvalue | nn:nn:nn:nn:nn:nn  | String  |
| ipvalue | A.B.C.D/A::B  | String  |


## show bgp l2vpn evpn route detail 

### Description 

```
Display Detailed Information 


```
### Syntax 

```
show bgp l2vpn evpn route detail

```
## show bgp l2vpn evpn route detail type 

### Description 

```
Specify Route type 


```
### Syntax 

```
show bgp l2vpn evpn route detail type { ead | es | macip | multicast | prefix }

```
## show bgp l2vpn evpn route type 

### Description 

```
Specify Route type 


```
### Syntax 

```
show bgp l2vpn evpn route type { ead | es | macip | multicast | prefix }

```
## show bgp l2vpn evpn summary 

### Description 

```
Summary of BGP neighbor status 


```
### Syntax 

```
show bgp l2vpn evpn summary

```
## show bgp l2vpn evpn vni 

### Description 

```
Show VNI 


```
### Syntax 

```
show bgp l2vpn evpn vni <vninum>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vninum | VNI  | Integer  |


## show image 

### Description 

```
Show image information 


```
### Syntax 

```
show image list

```
## show interface 

### Description 

```
Show Interface info 


```
### Syntax 

```
show interface { counters | { Ethernet [ <phy-if-id> ] } | { PortChannel [ <po-id> ] } | { Management [ <mgmt-if-id> ] } | { Vlan <vlan-id> } | { Loopback <lo-id> } | status }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-id | Unsigned integer  | String  |
| po-id |   | Integer  |
| mgmt-if-id |   | Integer  |
| vlan-id |   | Integer  |
| lo-id |   | Integer  |


## show ip access-group 

### Description 

```
Show IPv4 access-group information 


```
### Syntax 

```
show ip access-group

```
## show ip access-lists 

### Description 

```
Show IPv4 access-lists information 


```
### Syntax 

```
show ip access-lists [ <access-list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| access-list-name | String(Max: 63 characters)  | String  |


## show ip arp 

### Description 

```
show ARP commands 


```
### Syntax 

```
show ip arp [ <ip-addr> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip-addr | A.B.C.D  | String  |


## show ip arp interface 

### Description 

```
ARP entries for this interface 


```
### Syntax 

```
show ip arp interface { { Ethernet { <phy-if-name> [ summary ] } } | { Loopback { <lo-id> [ summary ] } } | { Management { <mgmt-if-id> [ summary ] } } | { PortChannel { <lag-id> [ summary ] } } | { Vlan { <vlan-id> [ summary ] } } | { Vxlan { <vxlan-if-name> [ summary ] } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-name | Unsigned integer  | String  |
| lo-id |   | Integer  |
| mgmt-if-id |   | Integer  |
| lag-id |   | Integer  |
| vlan-id |   | Integer  |
| vxlan-if-name | String(Max: 63 characters)  | String  |


## show ip arp mac-address 

### Description 

```
HW address 


```
### Syntax 

```
show ip arp mac-address <mac-addr>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |


## show ip arp summary 

### Description 

```
Summary of ARP entries 


```
### Syntax 

```
show ip arp summary

```
## show ip bgp 

### Description 

```
This command displays BGP information including routes, neighbors,
peer-group etc.


```
### Syntax 

```
show ip bgp { { [ ipv4 ] { { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | [ <prefix> ] | [ summary ] } } | { [ ipv6 ] { { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | [ <prefix> ] | [ summary ] } } | { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | { [ peer-group ] [ <peer-group-name> ] } | [ <prefix> ] | [ summary ] | { [ vrf ] { <vrf-name> { { [ ipv4 ] { { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | [ <prefix> ] | [ summary ] } } | { [ ipv6 ] { { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | [ <prefix> ] | [ summary ] } } | { [ neighbors ] { { [ <neighbor-ip> ] { [ routes ] | [ received-routes ] | [ advertised-routes ] } } | { [ interface ] { Ethernet | PortChannel | Vlan } { [ routes ] | [ received-routes ] | [ advertised-routes ] } } } } | { [ peer-group ] [ <peer-group-name> ] } | [ <prefix> ] | [ summary ] } } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| neighbor-ip | A.B.C.D/A::B  | String  |
| prefix | A.B.C.D/mask  | String  |
| peer-group-name | String  | String  |
| vrf-name | String(Max: 15 characters)  | String  |


### Usage Guidelines 

```
Use this command to display BGP neighbors, routes, peer-group etc. There
are various CLI options available to display various informations from
BGP. User can use "vrf" option to display information from a particular
VRF instance of BGP. User can also choose ipv4 or ipv6 to display
information from either of the address family.
- show ip bgp summary
This command will display BGP global parameters as well as brief
information about BGP neighbors
- show ip bgp
This command will show BGP local RIB routes. User can use filtering
options on CLI to zoom into a subset of routes that user is interested
in
- show ip bgp neighbor
This will display one or all BGP neighbors information in detail
- show ip bgp peer-group
This will display one or all BGP peer-group information in detail


```
### Examples 
#### Below are some of the sample outputs of show ip bgp          command 

```
leaf4# show ip bgp summary
BGP router identifier 200.9.0.5, local AS number 100
Neighbor        V   AS    MsgRcvd   MsgSent   InQ     OutQ    Up/Down  State/PfxRcd
14.14.14.1      4   400   8         2         0       0       00:00:43 0

leaf4# show ip bgp
BGP routing table information for VRF default
Router identifier 200.9.0.5, local AS number 100
Route status codes: * - valid, > - best
Origin codes: i - IGP, e - EGP, ? - incomplete
     Network             Next Hop            Metric         LocPref Path
*>   4.4.4.44/32         14.14.14.1          0                      400 ?
*>   10.59.128.0/20      14.14.14.1          0                      400 ?
*>   13.1.1.0/24         14.14.14.1          0                      400 ?
*>   14.14.14.0/24       14.14.14.1          0                      400 ?
*>   29.2.2.2/32         14.14.14.1          0                      400 ?
*>   192.168.1.0/24      14.14.14.1          0                      400 ?
*>   200.0.0.0/24        14.14.14.1          0                      400 ?

leaf4# show ip bgp neighbors

BGP neighbor is 14.14.14.1, remote AS 400, local AS 100, external link
  Administratively shut down
  BGP version 4, remote router ID  , local router ID
  BGP state = ESTABLISHED, up for 00:01:03
  Hold time is  seconds, keepalive interval is 60 seconds, negotiated hold time is 180 seconds
  Minimum time between advertisement runs is  seconds
  Neighbor capabilities:
    4 Byte AS: advertised and received
  Message statistics:
    InQ depth is 0
    OutQ depth is 0
                          Sent        Rcvd
    Opens:                1           1
    Notifications:        0           0
    Updates:              2           8
    Keepalive:            2           2
    Route Refresh:        0           0
    Capability:           0           0
    Total:                5           11

  Local host: 14.14.14.4, Local port: 46782
  Foreign host: 14.14.14.1, Foreign port: 179


```
## show ip igmp 

### Description 

```
Show IGMP snooping configuration across all the VLANs or specified VLAN Or
Show IGMP snooping groups learnt across all VLANs or specified VLAN


```
### Syntax 

```
show ip igmp snooping { { [ vlan ] <vlan-id> } { [ groups ] { [ vlan ] <vlan-id> } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id |   | Integer  |


### Usage Guidelines 

```
sonic# show ip igmp snooping
sonic# show ip igmp snooping groups


```
### Examples 
#### show IGMP Snooping information  

```
sonic# show ip igmp snooping
Vlan ID: 100
Querier: Disabled
IGMP Operation mode: IGMPv1
Is Fast-Leave Enabled: Disabled
Query interval: 125
Last Member Query Interval: 1000
Max Response time: 10

Vlan ID: 200
Querier: Enabled
IGMP Operation mode: IGMPv2
Is Fast-Leave Enabled: Disabled
Query interval: 125
Last Member Query Interval: 1000
Max Response time: 10

Vlan ID: 300
Querier: Enabled
IGMP Operation mode: IGMPv3
Is Fast-Leave Enabled: Disabled
Query interval: 20
Last Member Query Interval: 1000
Max Response time: 10


sonic# show ip igmp snooping vlan 200
Vlan ID: 200
Querier: Enabled
IGMP Operation mode: IGMPv2
Is Fast-Leave Enabled: Disabled
Query interval: 125
Last Member Query Interval: 1000
Max Response time: 10



```
#### show IGMP Snooping group information  

```
sonic# show ip igmp snooping groups
Vlan ID: 100
-----------
1 (*, 225.1.1.1)
  Outgoing Ports: Ethernet4,PortChannel3
2 (*, 225.1.1.2)
  Outgoing Ports: Ethernet8
Total number of entries: 2

Vlan ID : 300
-------------
1 (100.10.2.3, 226.0.0.1 )
  Outgoing Ports: Ethernet8,Portchannel2
Total number of entries: 1


sonic# show ip igmp snooping groups vlan 100
Vlan ID: 100
-----------
1 (*, 225.1.1.1)
  Outgoing Ports: Ethernet4, PortChannel3
2 (*, 225.1.1.2)
  Outgoing Ports: Ethernet8
Total number of entries: 2



```
## show ip interfaces 

### Description 

```
IP Info of Interfaces 


```
### Syntax 

```
show ip interfaces

```
## show ip prefix-list 

### Description 

```
IPv4 prefix list 


```
### Syntax 

```
show ip prefix-list [ <list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| list-name | String  | String  |


## show ip route 

### Description 

```
IP route information 


```
### Syntax 

```
show ip route { { [ vrf ] { <vrfname> [ <prefix> ] } } | [ <prefix> ] }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrfname | String  | String  |
| prefix | A.B.C.D/mask  | String  |


## show ip static-anycast-gateway 

### Description 

```
Displays IPv4 static-anycast-gateway information.


```
### Syntax 

```
show ip static-anycast-gateway

```
## show ip vrf 

### Description 

```
Show VRF information 


```
### Syntax 

```
show ip vrf [ <vrf-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrf-name | String(Max: 15 characters)  | String  |


## show ip vrf management 

### Description 

```
Show management VRF information 


```
### Syntax 

```
show ip vrf management

```
## show ipv6 interfaces 

### Description 

```
IPv6 Info of Interfaces 


```
### Syntax 

```
show ipv6 interfaces

```
## show ipv6 neighbors 

### Description 

```
show IPv6 neighbors commands 


```
### Syntax 

```
show ipv6 neighbors [ <ipv6-addr> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ipv6-addr | A::B  | String  |


## show ipv6 neighbors interface 

### Description 

```
neighbors entries for this interface 


```
### Syntax 

```
show ipv6 neighbors interface <if-type> { <if-id> [ summary ] }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| if-type | Interface type  | Select [Ethernet Vlan PortChannel Management(eth) ]  |
| if-id | Unsigned integer  | String  |


## show ipv6 neighbors mac-address 

### Description 

```
HW address 


```
### Syntax 

```
show ipv6 neighbors mac-address <mac-addr>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |


## show ipv6 neighbors summary 

### Description 

```
Summary of neighbors entries 


```
### Syntax 

```
show ipv6 neighbors summary

```
## show ipv6 prefix-list 

### Description 

```
IPv6 prefix list 


```
### Syntax 

```
show ipv6 prefix-list [ <list-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| list-name | String  | String  |


## show ipv6 route 

### Description 

```
IP route information 


```
### Syntax 

```
show ipv6 route { { [ vrf ] { <vrfname> [ <prefix> ] } } | [ <prefix> ] }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vrfname | String  | String  |
| prefix | A::B/mask  | String  |


## show ipv6 static-anycast-gateway 

### Description 

```
Displays IPv6 static-anycast-gateway information.


```
### Syntax 

```
show ipv6 static-anycast-gateway

```
## show kdump files 

### Description 

```
Show the kdump kernel core dump files which are stored locally.


```
### Syntax 

```
show kdump files

```
### Usage Guidelines 

```
Use this command to show the kdump kernel core dump files which are stored
locally.


```
### Examples 

```
sonic# show kdump files
Record Key           Filename
-------------------------------------------------------------
     1 202002101809 /var/crash/202002101809/dmesg.202002101809
                    /var/crash/202002101809/kdump.202002101809


```
## show kdump log 

### Description 

```
Show a kdump kernel core dump file kernel log from a file stored locally.


```
### Syntax 

```
show kdump log <record> [ <lines> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| record | kdump dump file record number  | Integer  |
| lines | Number of lines retrieved from kernel log file  | Integer  |


### Usage Guidelines 

```
Use this command to show a kdump kernel core dump file kernel log from a file
stored locally. The mandatory parameter is the number of the kernel core dump
files which are stored locally. The optional parameter is the number of lines
displayed (20 is the default number of lines displayed).


```
### Examples 

```
sonic# show kdump log 1 5
File: /var/crash/202002101809/dmesg.202002101809
[326785.222049]  [<ffffffffa0c0484e>] ? entry_SYSCALL_64_after_swapgs+0x58/0xc6
[326785.229926] Code: 41 5c 41 5d 41 5e 41 5f e9 6c 2f cf ff 66 2e 0f 1f 84 00 00 00 00 00 66 90 0f 1f 44 00 00 c7 05 29 28 a8 00 01 00 00 00 0f ae f8 <c6> 04 25 00 00 00 00 01 c3 0f 1f 44 00 00 0f 1f 44 00 00 53 8d
[326785.251451] RIP  [<ffffffffa0a2a562>] sysrq_handle_crash+0x12/0x20
[326785.258463]  RSP <ffffafd2c6523e78>
[326785.262453] CR2: 0000000000000000

In this example, we show the kernel log for the first kernel core dump file
stored locally. We display only the first 5 lines of the log.


```
## show kdump memory 

### Description 

```
Show the amount of memory reserved for kdump operation.


```
### Syntax 

```
show kdump memory

```
### Usage Guidelines 

```
Use this command to show the amount of memory reserved for kdump operation.


```
### Examples 

```
sonic# show kdump memory
Memory Reserved: 0M-2G:256M,2G-4G:320M,4G-8G:384M,8G-:448M


```
## show kdump num_dumps 

### Description 

```
Show the maximum number of kernel core dump files which can be stored locally.


```
### Syntax 

```
show kdump num_dumps

```
### Usage Guidelines 

```
Use this command to show the maximum number of kernel core dump files which
can be stored locally.


```
### Examples 

```
sonic# show kdump num_dumps
Maximum number of Kernel Core files Stored: 3


```
## show kdump status 

### Description 

```
Show the status of kdump operation.


```
### Syntax 

```
show kdump status

```
### Usage Guidelines 

```
Use this command to show the status of kdump operation.


```
### Examples 

```
sonic# show kdump status
Kdump Administrative Mode:  Enabled
Kdump Operational State:    Ready
Memory Reserved: 512M
Maximum number of Kernel Core files Stored: 3
Record Key           Filename
-------------------------------------------------------------
     1 202002101809 /var/crash/202002101809/dmesg.202002101809
                    /var/crash/202002101809/kdump.202002101809


```
## show link state tracking 

### Description 

```
Show link state tracking information 


```
### Syntax 

```
show link state tracking [ <grp-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-name | String(Max: 63 characters)  | String  |


## show lldp 

### Description 

```
Show lldp information 


```
### Syntax 

```
show lldp

```
## show lldp neighbor 

### Description 

```
Shows LLPD neigbhor information in detail


```
### Syntax 

```
show lldp neighbor [ <ifname> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ifname | String  | String  |


### Usage Guidelines 

```
This command is useful to view the LLDP neighbor information in detail


```
### Examples 
#### Shows LLDP neigbhor information in detail 

```
sonic-cli# show lldp neighbor
-----------------------------------------------------------
LLDP Neighbors
-----------------------------------------------------------
Interface:   Ethernet64,via: LLDP
Chassis:
    ChassisID:    80:a2:35:26:48:5e
    SysName:      Leaf9
    SysDescr:     Debian GNU/Linux 9 (stretch) Linux 4.9.0-11-2-amd64 #1 SMP Debian 4.9.189-3+deb9u2 (2019-11-11) x86_64
    MgmtIP:       10.59.132.165
    MgmtIP:       10.59.132.165
    Capability:   MAC_BRIDGE, ON
    Capability:   ROUTER, ON
Port
    PortID:       hundredGigE53
    PortDescr:    Ethernet64
-----------------------------------------------------------


```
## show lldp table 

### Description 

```
Shows LLPD neigbhor information in brief


```
### Syntax 

```
show lldp table

```
### Usage Guidelines 

```
This command is useful to view the LLDP neighbor information in brief


```
### Examples 
#### Shows LLDP neigbhor information in brief 

```
sonic-cli# show lldp table
------------------------------------------------------------------------------------------------------
LocalPort           RemoteDevice        RemotePortID        Capability           RemotePortDescr
-------------------------------------------------------------------------------------------------------
Ethernet64          Leaf9               hundredGigE53       BR                  Ethernet64


```
## show mac address-table 

### Description 

```
MAC address table 


```
### Syntax 

```
show mac address-table

```
## show mac address-table Vlan 

### Description 

```
Show MAC address-table for VLAN 


```
### Syntax 

```
show mac address-table Vlan <vlan-id>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id |   | Integer  |


## show mac address-table address 

### Description 

```
Show MAC address table address for MAC address 


```
### Syntax 

```
show mac address-table address <mac-addr>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |


## show mac address-table count 

### Description 

```
Count keyword 


```
### Syntax 

```
show mac address-table count

```
## show mac address-table dynamic 

### Description 

```
MAC address-table for dynamic commands 


```
### Syntax 

```
show mac address-table dynamic { { [ address ] <mac-addr> } | { [ Vlan ] <vlan-id> } | { [ interface ] { { Ethernet <phy-if-id> } | { PortChannel <port-channel-id> } } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |
| vlan-id |   | Integer  |
| phy-if-id | Unsigned integer  | String  |
| port-channel-id |   | Integer  |


## show mac address-table interface 

### Description 

```
Show MAC address-table for interfaces 


```
### Syntax 

```
show mac address-table interface { { Ethernet <phy-if-id> } | { PortChannel <port-channel-id> } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| phy-if-id | Unsigned integer  | String  |
| port-channel-id |   | Integer  |


## show mac address-table static 

### Description 

```
MAC address-table for static commands 


```
### Syntax 

```
show mac address-table static { { [ address ] <mac-addr> } | { [ Vlan ] <vlan-id> } | { [ interface ] { { Ethernet <phy-if-id> } | { PortChannel <port-channel-id> } } } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| mac-addr | nn:nn:nn:nn:nn:nn  | String  |
| vlan-id |   | Integer  |
| phy-if-id | Unsigned integer  | String  |
| port-channel-id |   | Integer  |


## show mclag brief 

### Description 

```
Show mclag domain/interface information 


```
### Syntax 

```
show mclag brief

```
## show mclag interface 

### Description 

```
Show mclag interface information 


```
### Syntax 

```
show mclag interface <ifid> <domain_id>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ifid |   | Integer  |
| domain_id |   | Integer  |


## show mirror-session 

### Description 

```
Display configured mirror sessions


```
### Syntax 

```
show mirror-session [ <session-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| session-name | String  | String  |


### Examples 

```
sonic# show mirror-session
ERSPAN Sessions
---------------------------------------------------------------------------------------------------------------
Name      Status    SRC-IP          DST-IP          GRE    DSCP  TTL   Queue   Policer   SRC-Port        Direction
---------------------------------------------------------------------------------------------------------------
Mirror2   active    11.1.1.1        10.1.1.1        0x88ee 10    10    10                Ethernet4       rx
SPAN Sessions
---------------------------------------------------------------
Name      Status    DST-Port        SRC-Port        Direction
---------------------------------------------------------------
Mirror1   active    Ethernet0       Ethernet4       rx


```
## show platform 

### Description 

```
Show platform information 


```
### Syntax 

```
show platform

```
## show platform environment 

### Description 

```
Show platform Environment 


```
### Syntax 

```
show platform environment

```
## show platform syseeprom 

### Description 

```
Show platoform eeprom information 


```
### Syntax 

```
show platform syseeprom

```
## show ptp 

### Description 

```
Display PTP status/configuration


```
### Syntax 

```
show ptp

```
### Examples 

```
sonic# show ptp
-----------------------------------------------------------
Interface            State
-----------------------------------------------------------
Ethernet56           master
Ethernet64           slave


```
## show ptp clock 

### Description 

```
Display PTP clock configuration/status


```
### Syntax 

```
show ptp clock

```
### Examples 

```
sonic# show ptp clock
Mode                  BC
Domain Profile        ieee1588
Network Transport     UDPv4 unicast
Domain Number         1
Clock Identity        3c2c99.fffe.2d7c35
Priority1             128
Priority2             128
Two Step              Enabled
Slave Only            False
Number Ports          2
Clock Quality:
Clock Class         248
Clock Accuracy      254
Ofst Scaled Log Var 65535
Mean Path Delay       0
Steps Removed         0
Offset from master    0


```
## show ptp parent 

### Description 

```
Display PTP parent status


```
### Syntax 

```
show ptp parent

```
### Examples 

```
sonic# show ptp parent
Parent Clock Identity          3c2c99.fffe.2d7c35
Port Number                    0
Grandmaster Clock Class        248
Grandmaster Off Scaled Log Var 65535
Grandmaster Clock Accuracy     254
Grandmaster Identity           3c2c99.fffe.2d7c35
Grandmaster Priority1          128
Grandmaster Priority2          128
Stats Valid                    False
Observed Off Scaled Log Var    65535
Observed Clock Phase Chg Rate  2147483647


```
## show ptp port 

### Description 

```
Display PTP port status/configuration


```
### Syntax 

```
show ptp port { Ethernet <ptp_port_number> }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| ptp_port_number | Unsigned integer  | String  |


### Examples 

```
sonic# show ptp port Ethernet 64
Port Number                    64
Port State                     master
Log Min delay Req Intvl        0
Peer Mean Path Delay           0
Log Announce Interval          1
Log Sync Interval              0
Log Min PDelay Req Interval    0
Version Number                 2
Unicast Master Table:
                               10.1.1.1


```
## show ptp time-property 

### Description 

```
Display PTP time-property status


```
### Syntax 

```
show ptp time-property

```
### Examples 

```
sonic# show ptp time-property
Curr UTC Offset Vld  False
Curr UTC Offset      37
Leap59               False
Leap61               False
Time Traceable       False
Freq Traceable       False
PTP Timescale        True


```
## show radius-server 

### Description 

```
Show RADIUS information 


```
### Syntax 

```
show radius-server

```
## show route-map 

### Description 

```
Display route map information 


```
### Syntax 

```
show route-map [ <rt-map-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| rt-map-name | String(Max: 63 characters)  | String  |


## show sample 

### Description 

```
Show all configured samples with their sampling rates.


```
### Syntax 

```
show sample <sample-name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| sample-name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Show all configured samples with their sampling rates.


```
### Examples 
#### Show sampling configuration 

```
sonic# show sample all
------------------------------------------------------------------------------------------------
SAMPLE NAME    SAMPLE RATE
------------------------------------------------------------------------------------------------
s1             200
s2             5000
sonic# show sample s1
------------------------------------------------------------------------------------------------
SAMPLE NAME    SAMPLE RATE
------------------------------------------------------------------------------------------------
s1             200



```
## show sflow 

### Description 

```
Show global sFlow configuration

```
### Syntax 

```
show sflow

```
### Examples 

```
sonic# show sflow
---------------------------------------------------------
Global sFlow Information
---------------------------------------------------------
admin state:       up
polling-interval:  20
agent-id:          default
sonic#


```
## show sflow interface 

### Description 

```
Show sFlow interface configuration

```
### Syntax 

```
show sflow interface

```
### Examples 

```
sonic# show sflow interface
-----------------------------------------------------------
sFlow interface configurations
Interface            Admin State             Sampling Rate
Ethernet0            up                      4000
Ethernet1            up                      4000
Ethernet2            up                      4000
Ethernet3            up                      4000
Ethernet4            up                      4000
Ethernet5            up                      4000
Ethernet6            up                      4000
Ethernet7            up                      4000
Ethernet8            up                      4000
Ethernet9            up                      4000
Ethernet10           up                      4000
Ethernet11           up                      4000
Ethernet12           up                      4000
Ethernet13           up                      4000
Ethernet14           up                      4000
Ethernet15           up                      4000
Ethernet16           up                      4000
Ethernet17           up                      4000
Ethernet18           up                      4000
Ethernet19           up                      4000
Ethernet20           up                      4000
Ethernet21           up                      4000
--more--
Ethernet22           up                      4000
Ethernet23           up                      4000
Ethernet24           up                      4000
Ethernet25           up                      4000
Ethernet26           up                      4000
Ethernet27           up                      4000
Ethernet28           up                      4000
Ethernet29           up                      4000
sonic#


```
## show snmp-server 

### Description 

```
Displays the Simple Network Management Protocol (SNMP) server information including
the physical location of the switch, the organization responsible for the network,
SNMP engine identification, trap status and the agent addresses, if configured.
SNMP engine identification is derived from the device MAC address on an initial boot.


```
### Syntax 

```
show snmp-server

```
### Usage Guidelines 

```
Use this command to view global SNMP server information.


```
### Examples 

```
sonic# show snmp-server

Location   : Lab1, Rack-10
Contact    : Broadcom Support
EngineID   : 8000013703525400f6817e
Traps      : enable

Agent Addresses:

               IP Address               UDP Port            Interface
--------------------------------------- -------- --------------------------------
1.2.3.4                                 161
1.2.3.4                                 1024
1.2.3.5                                 1024     Ethernet10


```
## show snmp-server community 

### Description 

```
Displays the SNMP communities configured on the switch and the community group
association, if configured. Communities are used by SNMPv2 protocol to access the switch.


```
### Syntax 

```
show snmp-server community

```
### Usage Guidelines 

```
Use this command to view the configured SNMP communities.


```
### Examples 

```
sonic# show snmp-server community

         Community Name                     Group Name
-------------------------------- --------------------------------
comm1                            group-lab
comm2                            None


```
## show snmp-server group 

### Description 

```
Displays the SNMP groups configured on the switch. The model and security information
indicate the SNMP protocol and security level used to access the system via the group.
View names indicate the view that a group provides read, write or trap access to.


```
### Syntax 

```
show snmp-server group

```
### Usage Guidelines 

```
Use this command to view the configured SNMP groups.


```
### Examples 

```
sonic# show snmp-server group

   Group Name      Model: Security       Read View        Write View      Notify View
---------------- -------------------- ---------------- ---------------- ----------------
group-floor1     v2c: no-auth-no-priv ro_view          wr_view          None
group-floor2     v3 : auth-priv       r_view           None             None
group-lab        v2c: no-auth-no-priv None             None             None


```
## show snmp-server host 

### Description 

```
Displays the SNMP hosts to which the trap or inform messages are sent by the SNMP agent.
Timeout indicates the number of seconds before the traps/informs time out when sending to a host.
Retries indicate the number of times the traps/informs are sent after timing out.


```
### Syntax 

```
show snmp-server host

```
### Usage Guidelines 

```
Use this command to view the configured SNMP hosts.


```
### Examples 

```
sonic# show snmp-server host

             Target Address              Type    Community    Ver T-Out Retries
--------------------------------------- ------ -------------- --- ----- -------
1.2.3.4                                 trap   comm1          v2c 15    3


             Target Address              Type    User Name        Security    T-Out Retries
--------------------------------------- ------ -------------- --------------- ----- -------
1001::1                                 inform user1          auth-priv       200   10


```
## show snmp-server user 

### Description 

```
Displays the SNMPv3 users configured on the switch including any authentication
and/or encryption algorithm for the user. The group name indicates a group
that defines the SNMPv3 access parameters.


```
### Syntax 

```
show snmp-server user

```
### Usage Guidelines 

```
Use this command to view the configured SNMPv3 users.


```
### Examples 

```
sonic# show snmp-server user

           User Name                        Group Name            Auth  Privacy
-------------------------------- -------------------------------- ----- -------
user1                            group-lab                        md5   aes-128
user2                            group-floor2                     None  None


```
## show snmp-server view 

### Description 

```
Displays the SNMP views configured on the switch including the OID tree that
the view includes or excludes.


```
### Syntax 

```
show snmp-server view

```
### Usage Guidelines 

```
Use this command to view the configured SNMP views.


```
### Examples 

```
sonic# show snmp-server view

           View Name                         OID Tree               Type
-------------------------------- -------------------------------- --------
view1                            1.2.3.4.5.6.7.8.9.1              included
view2                            1.2.3.4.5.6.7.8.9.5.1            excluded


```
## show spanning-tree 

### Description 

```
Shows spanning-tree information


```
### Syntax 

```
show spanning-tree [ vlan ] { <vlan-id> { [ interface ] <name> } }

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id | VLAN ID  | Integer  |
| name | String  | String  |


### Usage Guidelines 

```
This command is useful in viewing the spanning-tree information


```
### Examples 
#### Shows spanning-tree 

```
Spanning-tree Mode: PVST

VLAN 100 - STP instance 0
------------------------------------------------------------------------------------------------------------
STP Bridge Parameters:

Bridge            Bridge    Bridge    Bridge    Hold  LastTopology  Topology
Identifier        MaxAge    Hello     FwdDly    Time  Change        Change
hex               sec       sec       sec       sec   sec           cnt
80643c2c99a704a0  20        2         15        1     515           4

RootBridge        RootPath  DesignatedBridge  Root        Max  Hel  Fwd
Identifier        Cost      Identifier        Port        Age  lo   Dly
hex                         hex                           sec  sec  sec
00646cb9c51613ca  1600      10643c2c992d8235  PortChannel120   2    15

STP Port Parameters:
Port            Prio Path      Port Uplink BPDU   State      Designated Designated       Designated
Num             rity Cost      Fast Fast   Filter            Cost       Root             bridge
PortChannel1    128  800       N    N      N      FORWARDING 800        00646cb9c51613ca 10643c2c992d8235


```
## show spanning-tree bpdu-guard 

### Description 

```
Shows spanning-tree BPDU guard information


```
### Syntax 

```
show spanning-tree bpdu-guard

```
### Usage Guidelines 

```
This command is useful in viewing the spanning-tree BPDU guard information for the ports


```
### Examples 
#### Shows spanning-tree bpdu-guard 

```
sonic#show spanning-tree bpdu-guard
PortNum         Shutdown    Port shut
                Configured  due to BPDU guard
Ethernet64       Y           N
PortChannel2     Y           N


```
## show spanning-tree counters 

### Description 

```
Shows spanning-tree counters information


```
### Syntax 

```
show spanning-tree counters [ vlan ] <vlan-id>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id | VLAN ID  | Integer  |


### Usage Guidelines 

```
This command is useful in viewing the spanning-tree counters information


```
### Examples 
#### Shows spanning-tree counters 

```
sonic(config)# do show spanning-tree counters

VLAN 100 - STP instance 0
----------------------------------------------------------------------
PortNum         BPDU Tx   BPDU Rx   TCN Tx    TCN Rx

----------------------------------------------------------------------
Ethernet0       0         0         0         0
Ethernet48      53        7         1         0
Ethernet62      0         0         0         0
Ethernet64      0         0         0         0
PortChannel1    0         76        1         0
PortChannel2    0         0         0         0
PortChannel3    0         0         0         0


```
## show spanning-tree inconsistentports 

### Description 

```
Shows spanning-tree root inconsistent information


```
### Syntax 

```
show spanning-tree inconsistentports [ vlan ] <vlan-id>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id | VLAN ID  | Integer  |


### Usage Guidelines 

```
This command is useful in viewing the spanning-tree root inconsistent ports information


```
### Examples 
#### Shows spanning-tree inconsistentports 

```
sonic# show spanning-tree inconsistentports

Root guard timeout: 30  secs

----------------------------------------------------------------------
PortNum          VLAN  Inconsistency State
----------------------------------------------------------------------
Ethernet48       100   Root Inconsistent (29 seconds left on timer)


```
## show system 

### Description 

```
Show system information 


```
### Syntax 

```
show system

```
## show system cpu 

### Description 

```
Show system cpu information 


```
### Syntax 

```
show system cpu

```
## show system memory 

### Description 

```
Show system memory information 


```
### Syntax 

```
show system memory

```
## show system processes 

### Description 

```
Show system processes information 


```
### Syntax 

```
show system processes

```
## show system processes pid 

### Description 

```
Show system process information of a particular PID 


```
### Syntax 

```
show system processes pid <pid-no>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| pid-no | Unsigned integer  | String  |


## show tacacs-server global 

### Description 

```
Show tacacs global configuration 


```
### Syntax 

```
show tacacs-server global

```
## show tacacs-server host 

### Description 

```
Show tacacs server configuration 


```
### Syntax 

```
show tacacs-server host [ <address> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| address | A.B.C.D  | String  |


## show tam collector 

### Description 

```
This command is used to show TAM collector information.


```
### Syntax 

```
show tam collector [ <name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
This command displays the configured TAM collector information.


```
### Examples 
#### Show TAM collector info 

```
sonic# show tam collector
------------------------------------------------------------------------------------------------
NAME           IP TYPE        IP ADDRESS     PORT
------------------------------------------------------------------------------------------------
c1             ipv4           3.3.3.3        7777


```
## show tam device 

### Description 

```
This command is used to show TAM device information.


```
### Syntax 

```
show tam device

```
### Usage Guidelines 

```
This command displays the configured TAM Device Identifier.


```
### Examples 
#### Show TAM info 

```
sonic# show tam device
---------------------------------------------------------
TAM Device Information
---------------------------------------------------------
device-id: 5000


```
## show tam drop-monitor aging-interval 

### Description 

```
This command is used to show the system-level drop-monitor aging interval configured.


```
### Syntax 

```
show tam drop-monitor aging-interval

```
### Usage Guidelines 

```
This command shows the system-level drop-monitor aging interval configured.


```
### Examples 
#### Show drop monitor aging interval 

```
sonic# show tam drop-monitor aging-interval
Aging interval : 6 seconds


```
## show tam drop-monitor flow 

### Description 

```
This command is used to show information about all the configured flows or a specific flow identified by flow-name.


```
### Syntax 

```
show tam drop-monitor flow [ <flow-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| flow-name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
All the configured drop-monitor flows and their corresponding flows are displayed.


```
### Examples 
#### Show drop monitor flow info 

```
sonic# show tam drop-monitor flow
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE        COLLECTOR       SAMPLE          FLOWGROUP ID
------------------------------------------------------------------------------------------------
f2             t2             r2              c1              s1              5
f3             t3             r3              c1              s1              6
f4             t4             r4              c1              s1              4

sonic# show tam drop-monitor flow f2
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE        COLLECTOR       SAMPLE          FLOWGROUP ID
------------------------------------------------------------------------------------------------
f2             t2             r2              c1              s1              5



```
## show tam drop-monitor statistics 

### Description 

```
This command is used to show per flow statistics for drop-monitor. These statistics indicate the number of packets matching the flow.


```
### Syntax 

```
show tam drop-monitor statistics [ <flow-name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| flow-name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Match statistics for the given flow are displayed by this command.


```
### Examples 
#### Show drop monitor statistics 

```
sonic# show tam drop-monitor statistics
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       PACKET COUNT   BYTE COUNT
------------------------------------------------------------------------------------------------
f2             t2             r2             0              0
f3             t3             r3             0              0
f4             t4             r4             0              0


```
## show tam drop-monitor supported 

### Description 

```
This command is used to determine if drop-monitor feature functionality is supported.


```
### Syntax 

```
show tam drop-monitor supported

```
### Usage Guidelines 

```
Use this command to check if drop monitor feature is supported.


```
### Examples 
#### Check if drop-monitor capability is supported 

```
sonic# show tam drop-monitor supported
Feature Supported      : True


```
## show tam int-ifa flow 

### Description 

```
Show IFA flow configuration.


```
### Syntax 

```
show tam int-ifa flow [ <name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Use this command to display IFA flow configuration.


```
### Examples 
#### IFA flow configuration 

```
sonic# show tam int-ifa flow
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       SAMPLING RATE  COLLECTOR
------------------------------------------------------------------------------------------------
iflow1         iacl1          irule1         12             icol
iflow2         iacl2          irule1         17             icol1

sonic# show tam int-ifa flow iflow2
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       SAMPLING RATE  COLLECTOR
------------------------------------------------------------------------------------------------
iflow2         iacl2          irule1         17             icol1



```
## show tam int-ifa statistics 

### Description 

```
Shows IFA flow statistics.


```
### Syntax 

```
show tam int-ifa statistics [ <name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Use this command to display packet count and byte count for matching IFA flow.


```
### Examples 
#### Display IFA flow statistics 

```
sonic# show tam int-ifa statistics all
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       PACKET COUNT   BYTE COUNT
------------------------------------------------------------------------------------------------
flow1          t1             r1             0              0
flow2          t2             r2             0              0
sonic# show tam int-ifa statistics flow1
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       PACKET COUNT   BYTE COUNT
------------------------------------------------------------------------------------------------
flow1          t1             r1             0


```
## show tam int-ifa status 

### Description 

```
Shows IFA overall status.


```
### Syntax 

```
show tam int-ifa status

```
### Usage Guidelines 

```
Use this command to display overall IFA status including device-id, number of collectors configured, number of flows configured etc.


```
### Examples 
#### Shows IFA overall status 

```
sonic# show tam int-ifa status
---------------------------------------------------------
TAM/IFA Status
---------------------------------------------------------
Device Identifier    : 7765
Number of collectors : 1
Number of flows      : 1
Feature Enabled      : True


```
## show tam int-ifa supported 

### Description 

```
Shows IFA feature status.


```
### Syntax 

```
show tam int-ifa supported

```
### Usage Guidelines 

```
Use this command to display IFA feature status.


```
### Examples 
#### Show IFA feature details 

```
sonic# show tam int-ifa supported
---------------------------------------------------------
TAM IFA Feature Information
---------------------------------------------------------
IFA Feature Supported: True


```
## show tam int-ifa-ts flow 

### Description 

```
Shows IFA Tail Timestamping flow configutaion details.


```
### Syntax 

```
show tam int-ifa-ts flow [ <name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Use this command to display flow configuration once flow configuration has been done.


```
### Examples 
#### Shows IFA Tail Timestamping flow details 

```
sonic# show tam int-ifa-ts flow all
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE
------------------------------------------------------------------------------------------------
flow1          t1             r1
flow2          t2             r2
sonic#
sonic#
sonic# show tam int-ifa-ts flow flow1
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE
------------------------------------------------------------------------------------------------
flow1          t1             r1


```
## show tam int-ifa-ts statistics 

### Description 

```
Shows IFA Tail Timestamping flow statistics


```
### Syntax 

```
show tam int-ifa-ts statistics [ <name> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| name | String(Max: 63 characters)  | String  |


### Usage Guidelines 

```
Use this command to dump tail timestamping flow statistics..


```
### Examples 
#### Shows IFA Tail Timestamping flow statistics 

```
sonic# show tam int-ifa-ts statistics all
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       PACKET COUNT   BYTE COUNT
------------------------------------------------------------------------------------------------
flow1          t1             r1             0              0
flow2          t2             r2             0              0
sonic# show tam int-ifa-ts statistics flow1
------------------------------------------------------------------------------------------------
FLOW           ACL TABLE      ACL RULE       PACKET COUNT   BYTE COUNT
------------------------------------------------------------------------------------------------
flow1          t1             r1             0              0


```
## show tam int-ifa-ts status 

### Description 

```
Shows IFA Tail Timestamping status.


```
### Syntax 

```
show tam int-ifa-ts status

```
### Usage Guidelines 

```
Use this command to display overall status of IFA Tail Timestamping feature.


```
### Examples 
#### Shows IFA Tail Timestamping status details 

```
sonic# show tam int-ifa-ts status
---------------------------------------------------------
TAM INT IFA TS Status
---------------------------------------------------------
Device Identifier    : 2345
Number of flows      : 2
Feature Enabled      : True



```
## show tam int-ifa-ts supported 

### Description 

```
Shows IFA Tail Timestamping feature status.


```
### Syntax 

```
show tam int-ifa-ts supported

```
### Usage Guidelines 

```
After enabling IFA Timestamping feature, use this command to display feature status.


```
### Examples 
#### Shows IFA Tail Timestamping feature enabled status 

```
sonic(config)# tam
sonic(config-tam)# int-ifa-ts
sonic(config-int-ifa-ts)# feature enable
sonic# show tam int-ifa-ts supported
Feature Supported      : True


```
## show tech-support 

### Description 

```
Collect technical support information 


```
### Syntax 

```
show tech-support [ since ] <date>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| date | String  | String  |


## show udld global 

### Description 

```
Shows global level UDLD information


```
### Syntax 

```
show udld global

```
### Usage Guidelines 

```
After enabling UDLD at global level or modifying global level UDLD attributes, use this command to check global level UDLD information


```
### Examples 
#### Shows UDLD global level details 

```
sonic-cli(config)# udld enable
sonic-cli# show udld global

UDLD Global Information
  Admin State        : UDLD Enabled
  Mode               : Normal
  UDLD Message Time  : 1 seconds
  UDLD Multiplier    : 3


```
## show udld interface 

### Description 

```
Shows interface level UDLD information and neighbors details on this interface


```
### Syntax 

```
show udld interface <interface-name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| interface-name | String  | String  |


### Usage Guidelines 

```
After enabling UDLD at interface level, use this command to get interface level UDLD information and neighbors attached to this interface.


```
### Examples 
#### Shows interface level UDLD information and neighbors details on this interface 

```
sonic-cli(config)# udld enable
sonic-cli(config)# interface Ethernet 0
sonic-cli(conf-if-Ethernet0)# udld enable
sonic-cli# show udld interface Ethernet0

UDLD information for Ethernet0
  UDLD Admin State:                  Enabled
  Mode:                              Normal
  Status:                            Bidirectional
  Local device id:                   3c2c.992d.8201
  Local port id :                    Ethernet0
  Local device name:                 Sonic
  Message time:                      1
  Timeout interval:                  3
    Neighbor Entry 1
    ----------------------------------------------------------------------------------------
    Neighbor device id:         3c2c.992d.8235
    Neighbor port id:           Ethernet0
    Neighbor device name:       Sonic
    Neighbor message time:      1
    Neighbor timeout interval:  3


```
## show udld neighbors 

### Description 

```
Shows UDLD neighbors information


```
### Syntax 

```
show udld neighbors

```
### Usage Guidelines 

```
After enabling UDLD at global and interface level, use this command to get all UDLD neighbors information.


```
### Examples 
#### Shows UDLD neighbors details 

```
sonic-cli(config)# udld enable
sonic-cli(config)# interface Ethernet 0
sonic-cli(conf-if-Ethernet0)# udld enable
sonic-cli# show udld neighbors

Port           Device Name     Device ID         Port ID         Neighbor State
---------------------------------------------------------------------------------
Ethernet1      Sonic           3c2c.992d.8201    Ethernet0       Bidirectional
Ethernet3      Sonic           3c2c.992d.8201    Ethernet3       Bidirectional


```
## show udld statistics 

### Description 

```
Shows UDLD statistics for all interfaces


```
### Syntax 

```
show udld statistics

```
### Usage Guidelines 

```
Use this command to get UDLD statistics for all interfaces


```
### Examples 
#### Shows UDLD statistics for all interfaces 

```
sonic-cli# show udld statistics

UDLD Interface statistics for Ethernet0
Frames transmitted:         10
Frames received:            9
Frames with error:          0

UDLD Interface statistics for Ethernet1
Frames transmitted:         5
Frames received:            8
Frames with error:          0


```
## show udld statistics interface 

### Description 

```
Shows UDLD statistics for a specific interface


```
### Syntax 

```
show udld statistics interface <interface-name>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| interface-name | String  | String  |


### Usage Guidelines 

```
Use this command to get UDLD statistics for a specific interface


```
### Examples 
#### Shows UDLD statistics for a specific interface 

```
sonic-cli# show udld statistics interface Ethernet0

UDLD Interface statistics for Ethernet0
Frames transmitted:         10
Frames received:            9
Frames with error:          0


```
## show version 

### Description 

```
Show version information 


```
### Syntax 

```
show version

```
## show vxlan interface 

### Description 

```
Show command to display the name, SIP, associated NVO name,
the loopback interface configured with the VTEP SIP.


```
### Syntax 

```
show vxlan interface

```
### Usage Guidelines 

```
sonic# show vxlan interface


```
### Examples 
#### show vxlan interface 

```
sonic# show vxlan interface

VTEP Information:

    VTEP Name : VTEP1, SIP  : 4.4.4.4
    NVO Name  : nvo1,  VTEP : VTEP1
    Source interface  : Loopback33


```
## show vxlan remote mac 

### Description 

```
Show command to display all the MACs learnt from the specified remote IP or all the remotes for the specified/all VLANs.
VLAN, MAC, RemoteVTEP, VNI, Type are the columns.


```
### Syntax 

```
show vxlan remote mac [ <remote_ip_addr> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| remote_ip_addr | A.B.C.D  | String  |


### Usage Guidelines 

```
sonic# show vxlan remote mac


```
### Examples 
#### show vxlan remote mac information 

```
sonic# show vxlan remote mac
+---------+-------------------+--------------+-------+--------+
| VLAN    | MAC               | RemoteVTEP   |   VNI | Type   |
+=========+===================+==============+=======+========+
| Vlan101 | 00:00:00:00:00:01 | 4.4.4.4      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:02 | 3.3.3.3      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:03 | 4.4.4.4      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:04 | 4.4.4.4      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:05 | 4.4.4.4      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:99 | 3.3.3.3      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
Total count : 6

sonic# show vxlan remote mac 3.3.3.3
+---------+-------------------+--------------+-------+--------+
| VLAN    | MAC               | RemoteVTEP   |   VNI | Type   |
+=========+===================+==============+=======+========+
| Vlan101 | 00:00:00:00:00:02 | 3.3.3.3      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
| Vlan101 | 00:00:00:00:00:99 | 3.3.3.3      |  1001 | static |
+---------+-------------------+--------------+-------+--------+
Total count : 2


```
## show vxlan remote vni 

### Description 

```
Show command to display all the VLANs learnt from the specified remote IP or all the remotes.
VLAN, RemoteVTEP, VNI are the columns


```
### Syntax 

```
show vxlan remote vni [ <remote_ip_addr> ]

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| remote_ip_addr | A.B.C.D  | String  |


### Usage Guidelines 

```
sonic# show vxlan remote vni


```
### Examples 
#### show vxlan remote vni information 

```
sonic# show vxlan remote vni

+---------+--------------+-------+
| VLAN    | RemoteVTEP   |   VNI |
+=========+==============+=======+
| Vlan101 | 3.3.3.3      |  1001 |
+---------+--------------+-------+
| Vlan101 | 4.4.4.4      |  1001 |
+---------+--------------+-------+
Total count : 2

sonic# show vxlan remote vni 3.3.3.3

+---------+--------------+-------+
| VLAN    | RemoteVTEP   |   VNI |
+=========+==============+=======+
| Vlan101 | 3.3.3.3      |  1001 |
+---------+--------------+-------+
Total count : 1


```
## show vxlan tunnel 

### Description 

```
Show command to display all the discovered tunnels.
SIP, DIP, Creation Source, OperStatus are the columns.


```
### Syntax 

```
show vxlan tunnel

```
### Usage Guidelines 

```
sonic# show vxlan tunnel


```
### Examples 
#### show vxlan tunnel 

```
sonic# show vxlan tunnel

+---------+---------+-------------------+--------------+
| SIP     | DIP     | Creation Source   | OperStatus   |
+=========+=========+===================+==============+
| 2.2.2.2 | 4.4.4.4 | EVPN              | oper_up      |
+---------+---------+-------------------+--------------+
| 2.2.2.2 | 3.3.3.3 | EVPN              | oper_up      |
+---------+---------+-------------------+--------------+
Total count : 2


```
## show vxlan vlanvnimap 

### Description 

```
Show command to display all the VLAN VNI mappings


```
### Syntax 

```
show vxlan vlanvnimap

```
### Usage Guidelines 

```
sonic# show vxlan vlanvnimap


```
### Examples 
#### show vxlan vlan-vni map 

```
sonic# show vxlan vlanvnimap

+---------+-------+
| VLAN    |   VNI |
+=========+=======+
| Vlan100 |   100 |
+---------+-------+
| Vlan101 |   101 |
+---------+-------+
Total count : 2


```
## show vxlan vrfvnimap 

### Description 

```
Show command to display all the VRF VNI mappings


```
### Syntax 

```
show vxlan vrfvnimap

```
### Usage Guidelines 

```
sonic# show vxlan vrfvnimap


```
### Examples 
#### show vxlan vrf-vni map 

```
sonic# show vxlan vrfvnimap

+-------+-------+
| VRF   |   VNI |
+=======+=======+
| Vrf1  |   600 |
+-------+-------+
Total count : 1


```
## show ztp-status 

### Description 

```
Show the status of ZTP operation.


```
### Syntax 

```
show ztp-status

```
### Usage Guidelines 

```
Use this command to show the status of ZTP operation.

These are the possible current states or result of ZTP session:
 - IN-PROGRESS: ZTP session is currently in progress. ZTP service is processing switch provisioning information.
 - SUCCESS: ZTP service has successfully processed the switch provisioning information.
 - FAILED: ZTP service has failed to process the switch provisioning information.
 - Not Started: ZTP service has not started processing the discovered switch provisioning information.

These are the state and result of a configuration section:
 - IN-PROGRESS: Corresponding configuration section is currently being processed.
 - SUCCESS: Corresponding configuration section was processed successfully.
 - FAILED: Corresponding configuration section failed to execute successfully.
 - Not Started: ZTP service has not started processing the corresponding configuration section.
 - DISABLED: Corresponding configuration section has been marked as disabled and will not be processed.



```
### Examples 

```
sonic# show ztp-status
========================================
ZTP
========================================
ZTP Admin Mode      : True
ZTP Service         : Inactive
ZTP Status          : Not Started


```
## shutdown 
### Description 
```
Shut Bidirectional Forwarding detection(BFD) peer administratively down.
```
### Parent Commands (Modes) 
```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>
```
### Syntax 
```
shutdown
no shutdown
```
### Usage Guidelines 
```
This command will change the BFD session state to DOWN.
```
### Examples 
#### Shut BFD peer down 
```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# shutdown
```
## shutdown 
### Description 
```
This command administratively shutsdown a BGP neighbor. The CLI allows
user to specify a shutdown message that can be communicated to the
neighbor
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
shutdown [ message ] <MSG>
no shutdown [ message ] <MSG>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| MSG | String  | String  |
### Usage Guidelines 
```
Use this command to administratively shutdown a BGP neighbor
sessions
```
### Examples 
#### Following command shutdown a neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# shutdown
```
## shutdown 
### Description 
```
This command administratively shutsdown a BGP peer-group. The CLI allows
user to specify a shutdown message that can be communicated to the
neighbors in peer-group
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
shutdown [ message ] <MSG>
no shutdown [ message ] <MSG>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| MSG | String  | String  |
### Usage Guidelines 
```
Use this command to administratively shutdown a BGP peer-group
sessions
```
### Examples 
#### Following command shutdown a peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# shutdown
```
## shutdown 
### Description 
```
Disable the interface 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
shutdown
no shutdown
```
## shutdown 
### Description 
```
Disable the interface 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
shutdown
no shutdown
```
## shutdown 
### Description 
```
Disable the interface 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
shutdown
no shutdown
```
## snmp-server agentaddress 
### Description 
```
Configure one or more SNMP agent addresses and optionally set the UDP port number on
which the SNMP server listens for requests, and the Virtual Routing and Forwarding (VRF)
interface used by the management station to access SNMP. The default UDP port is 161.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server agentaddress <host-addr> { { [ port ] <udp-port> } { [ interface ] <ifname> } }
no snmp-server agentaddress <host-addr> { { [ port ] <udp-port> } { [ interface ] <ifname> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| host-addr | A.B.C.D or A:B:C:D:E:F:G:H  | String  |
| udp-port |   | Integer  |
| ifname | String(Max: 32 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure an SNMP agent address, UDP port number, and VRF interface.
```
### Examples 
#### Add an SNMP agent address using the default UDP port number. 
```
sonic# configure terminal
sonic(config)# snmp-server agentaddress 1.2.3.4
```
#### Add an SNMP agent address specifying a non-default UDP port number. 
```
sonic# configure terminal
sonic(config)# snmp-server agentaddress 1.2.3.4 port 1024
```
#### Add an SNMP agent address specifying a non-default UDP port number and a VRF interface. 
```
sonic# configure terminal
sonic(config)# snmp-server agentaddress 1.2.3.5 port 1024 interface Ethernet10
```
## snmp-server community 
### Description 
```
Configure one or more SNMP communities and optionally associate them with a group.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server community <community-name> { [ group ] <group-name> }
no snmp-server community <community-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| community-name | String (Max: 32 characters)  | String  |
| group-name | String (Max: 32 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure an SNMP community and group.
```
### Examples 
#### Add an SNMP community without specifying a group. 
```
sonic# configure terminal
sonic(config)# snmp-server community comm1
```
#### Add an SNMP community and associate it with a group. 
```
sonic# configure terminal
sonic(config)# snmp-server community comm1 group group-lab
```
## snmp-server contact 
### Description 
```
Configure the contact information about the organization responsible for the network.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server contact <contact-name>
no snmp-server contact
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| contact-name | String  | String  |
### Usage Guidelines 
```
Use this command to configure the SNMP server contact information.
```
### Examples 
```
sonic# configure terminal
sonic(config)# snmp-server contact "Broadcom Support"
```
## snmp-server enable 
### Description 
```
Enable the SNMP authentication flag on the switch. The flag is disabled by default.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server enable trap
no snmp-server enable trap
```
### Usage Guidelines 
```
Use this command to configure the SNMP authentication flag.
```
### Examples 
```
sonic# configure terminal
sonic(config)# snmp-server enable trap
```
## snmp-server engine 
### Description 
```
Configure the SNMP engine identification on the local device. It is a hexadecimal
string used for localizing configuration. The default engine ID is derived from
the device MAC address.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server engine <engineID>
no snmp-server engine
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| engineID | Octet (hex) string, 5-32 octets  | String  |
### Usage Guidelines 
```
Use this command to configure the SNMP engine ID.
```
### Examples 
```
sonic# configure terminal
sonic(config)# snmp-server engine 8100013703525400abcd
```
## snmp-server group 
### Description 
```
Configure one or more SNMPv2c and SNMPv3 access groups and optionally set the views which
the group uses for the GET/SET requests and to send traps. Authentication and privacy can be
set for SNMPv3 groups only. Groups are used when configuring SNMP communities and users.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server group <group-name> { { any | v2c | { v3 { noauth | auth | priv } } } { [ read ] <read-view> } { [ write ] <write-view> } { [ notify ] <notify-view> } }
no snmp-server group <group-name> { any | v2c | { v3 { noauth | auth | priv } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| group-name | String (Max: 32 characters)  | String  |
| read-view | String (Max: 32 characters)  | String  |
| write-view | String (Max: 32 characters)  | String  |
| notify-view | String (Max: 32 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure an SNMP access group.
```
### Examples 
#### Add an SNMP group that can only access via SNMPv2c without associating it with a view. 
```
sonic# configure terminal
sonic(config)# snmp-server group group1 v2c
```
#### Add an SNMP group that can only access via SNMPv2c associating it with a view for only sending out traps. 
```
sonic# configure terminal
sonic(config)# snmp-server group group1 v2c notify no_view
```
#### Add an SNMP group that can only access via SNMPv3 specifying the security level and without associating it with a view. 
```
sonic# configure terminal
sonic(config)# snmp-server group group-floor2 v3 priv
```
#### Add an SNMP group that can only access via SNMPv3 associating it with the views for the GET/SET requests and sending out traps. 
```
sonic# configure terminal
sonic(config)# snmp-server group group-floor2 v3 priv read r_view write w_view notify n_view
```
## snmp-server host 
### Description 
```
Configure one or more SNMP IPv4 or IPv6 hosts to which the trap or inform messages are
sent to by the SNMP agent. Optionally set the timeout and number of retries for the inform
messages sent to a host. Timeout indicates the number of seconds before the informs time out
when sending to a host. Retries indicate the number of times the informs are sent after timing out.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server host <host-addr> { { community { <community-name> { { [ traps ] v2c } | { [ informs ] { [ timeout ] <time-out> } { [ retries ] <retry> } } } } } | { user { <username> { { [ traps ] { noauth | auth | priv } } | { [ informs ] { noauth | auth | priv } { [ timeout ] <time-out> } { [ retries ] <retry> } } } } } }
no snmp-server host <host-addr>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| host-addr | A.B.C.D or A:B:C:D:E:F:G:H  | String  |
| community-name | String (Max: 32 characters)  | String  |
| time-out |   | Integer  |
| retry |   | Integer  |
| username | String (Max: 32 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure an SNMP host.
```
### Examples 
#### Add an SNMP IPv4 host community to receive SNMPv2c traps. 
```
sonic# configure terminal
sonic(config)# snmp-server host 1.2.3.4 community comm1 traps v2c
```
#### Add an SNMP IPv4 host user to receive SNMPv3 informs without authentication specifying the timeout and number of retries. 
```
sonic# configure terminal
sonic(config)# snmp-server host 1.2.3.5 user user1 informs noauth timeout 200 retries 10
```
#### Add an SNMP IPv6 host community to receive SNMPv2c informs without authentication specifying the timeout and number of retries. 
```
sonic# configure terminal
sonic(config)# snmp-server host 2001::1 community comm2 informs timeout 150 retries 5
```
#### Add an SNMP IPv6 host user to receive SNMPv3 traps with authentication and privacy. 
```
sonic# configure terminal
sonic(config)# snmp-server host 3001::1 user u1 traps priv
```
## snmp-server location 
### Description 
```
Configure the physical location of the switch.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server location <location-name>
no snmp-server location
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| location-name | String  | String  |
### Usage Guidelines 
```
Use this command to configure the SNMP server location information.
```
### Examples 
```
sonic# configure terminal
sonic(config)# snmp-server location "Lab1, Rack-10"
```
## snmp-server user 
### Description 
```
Configure one or more SNMPv3 users and optionally set the authentication and group
association. Authentication passwords can be encrypted. If password encryption is desired,
it must be specified prior to setting the authentication type.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server user <username> { { [ group ] <group-name> } { { [ encrypted ] { auth { { md5 { auth-password { <authpassword> { [ priv ] { { des { priv-password <privpassword> } } | { aes-128 { priv-password <privpassword> } } } } } } } | { sha { auth-password { <authpassword> { [ priv ] { { des { priv-password <privpassword> } } | { aes-128 { priv-password <privpassword> } } } } } } } } } } | { [ auth ] { noauth | { md5 { auth-password { <authpassword> { [ priv ] { { des { priv-password <privpassword> } } | { aes-128 { priv-password <privpassword> } } } } } } } | { sha { auth-password { <authpassword> { [ priv ] { { des { priv-password <privpassword> } } | { aes-128 { priv-password <privpassword> } } } } } } } } } } }
no snmp-server user <username>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| username | String (Max: 32 characters)  | String  |
| group-name | String (Max: 32 characters)  | String  |
| authpassword | 16-byte Hex String  | String  |
| privpassword | 16-byte Hex String  | String  |
### Usage Guidelines 
```
Use this command to configure an SNMPv3 user.
```
### Examples 
#### Add an SNMPv3 user without authentication and group association. 
```
sonic# configure terminal
sonic(config)# snmp-server user user1
```
#### Add an SNMPv3 user without authentication associating it with a group. 
```
sonic# configure terminal
sonic(config)# snmp-server user user1 group group-lab
```
#### Add an SNMPv3 user specifying authentication and group association. 
```
sonic# configure terminal
sonic(config)# snmp-server user user1 group group-lab auth md5 auth-password pwd priv aes-128 priv-password pwd
```
#### Add an SNMPv3 user specifying encrypted authentication and group association. 
```
sonic# configure terminal
sonic(config)# snmp-server user user2 group group-floor2 encrypted auth sha auth-password abcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcd priv des priv-password abcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcdabcd
```
## snmp-server view 
### Description 
```
Configure one or more SNMP views and set the OID tree to include or exclude from the view.
SNMP views are used by the groups for the GET/SET requests and to send traps.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
snmp-server view <view-name> { <oid-tree> { included | excluded } }
no snmp-server view <view-name> <oid-tree>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| view-name | String (Max: 32 characters)  | String  |
| oid-tree | OID (Max: 255 characters)  | String  |
### Usage Guidelines 
```
Use this command to configure a SNMP view.
```
### Examples 
#### Add an SNMP view that excludes the OID tree. 
```
sonic# configure terminal
sonic(config)# snmp-server view view2 1.2.3.4.5.6.7.8.9.2 excluded
```
## soft-reconfiguration 
### Description 
```
This command enables soft-reconfiguration for a BGP neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
### Usage Guidelines 
```
Use this command to store routes received (RIB-In) from a BGP neighbor.
These stored routes could be used to refresh the Loc-RIB in future as
needed. If inbound policy changes, these stored routes will be used to
generate LocRIB after applying the modified inbound policy.
```
### Examples 
#### Following command enables soft reconfiguration for neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# soft-reconfiguration
```
## soft-reconfiguration 
### Description 
```
This command enables soft-reconfiguration for BGP neighbors in a
peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
### Usage Guidelines 
```
Use this command to store routes received (RIB-In) from BGP neighbors in
a peer-group. These stored routes could be used to refresh the Loc-RIB in
future as needed. If inbound policy changes, these stored routes will be used to
generate LocRIB after applying the modified inbound policy.
```
### Examples 
#### Following command enables soft reconfiguration for          neighbors in a peer-group 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# soft-reconfiguration
```
## soft-reconfiguration 
### Description 
```
Per neighbor soft reconfiguration 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
## soft-reconfiguration 
### Description 
```
Per neighbor soft reconfiguration 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
## soft-reconfiguration 
### Description 
```
Per neighbor soft reconfiguration 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
## soft-reconfiguration 
### Description 
```
Per neighbor soft reconfiguration 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
soft-reconfiguration inbound
no soft-reconfiguration inbound
```
## solo 
### Description 
```
This command is used to indicate that routes advertised by the peer
should not be reflected back to the peer. This command is only
meaningful when there is a single peer defined in the peer-group.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
solo
no solo
```
### Usage Guidelines 
```
Use this command to set a neighbor solo
```
### Examples 
#### Following command configures BGP neighbor          30.30.30.3 as solo 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# solo
```
## solo 
### Description 
```
This command is used to indicate that routes advertised by the peer
should not be reflected back to the peer. This command is only
meaningful when there is a single peer defined in the peer-group.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
solo
no solo
```
### Usage Guidelines 
```
Use this command to set a peer-group solo
```
### Examples 
#### Following command configures BGP peer-group          PG_Ext as solo 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# solo
```
## source-ip 
### Description 
```
Set mclag source IPv4 address 
```
### Parent Commands (Modes) 
```
mclag domain <mclag-domain-id>
```
### Syntax 
```
source-ip <SIP>
no source-ip
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| SIP | A.B.C.D  | String  |
## source-ip 
### Description 
```
Command to set the source IPv4 address
```
### Parent Commands (Modes) 
```
interface Vxlan <vxlan-if-name>
```
### Syntax 
```
source-ip <SIP>
no source-ip
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| SIP | A.B.C.D  | String  |
### Usage Guidelines 
```
(conf-if-Vxlan-vtep)# source-ip SOURCEIP
SOURCEIP - source IPv4 address
```
### Examples 
#### configure the source IPv4 address 
```
sonic(config)# interface Vxlan vtep1
sonic(conf-if-Vxlan-vtep1)# source-ip 1.1.1.1
```
## source-vtep 
### Description 
```
Command to set the VxLAN interface to source the IP address
```
### Parent Commands (Modes) 
```
evpn <evpn_name>
```
### Syntax 
```
source-vtep <vxlan_name>
no source-vtep
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vxlan_name | String(Max: 63 characters)  | String  |
### Usage Guidelines 
```
(config-if-evpn)# source-vtep VTEPNAME
VTEPNAME - String
```
### Examples 
#### set vxlan interface to source the IP address 
```
sonic(config)# evpn evpn1
sonic(config-if-evpn)# source-vtep vtep1
```
## spanning-tree 
### Description 
```
Configure interface specific spanning-tree parameters.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
spanning-tree { { bpduguard [ port-shutdown ] } | { cost <value> } | enable | { link-type { point-to-point | shared } } | portfast | { port-priority <value> } | { port { type edge } } | uplinkfast }
no spanning-tree { bpdufilter | { bpduguard [ port-shutdown ] } | cost | enable | link-type | portfast | port-priority | { port type } | uplinkfast }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |
### Usage Guidelines 
```
These commands allow configuring interface specific spanning-tree parameters
```
### Examples 
```
sonic(config)# interface Ethernet 0
sonic(conf-if-Ethernet0)# spanning-tree bpduguard port-shutdown
sonic(conf-if-Ethernet0)# spanning-tree cost 1000
sonic(conf-if-Ethernet0)# spanning-tree enable
sonic(conf-if-Ethernet0)# spanning-tree portfast
sonic(conf-if-Ethernet0)# spanning-tree port-priority 16
sonic(conf-if-Ethernet0)# spanning-tree uplinkfast
sonic(conf-if-Ethernet0)# spanning-tree link-type point-to-point
sonic(conf-if-Ethernet0)# spanning-tree port type edge
```
## spanning-tree bpdufilter 

### Description 

```
Configure interface specific bpdu-filter parameters.


```
### Parent Commands (Modes) 

```
interface <phy-if-name>

```
### Syntax 

```
spanning-tree bpdufilter { enable | disable }

```
### Usage Guidelines 

```
These commands allow configuring interface specific bpdu-filter parameters


```
### Examples 

```
sonic(config)# interface Ethernet 0
sonic(conf-if-Ethernet0)# spanning-tree bpdufilter enable
sonic(conf-if-Ethernet0)# spanning-tree bpdufilter disable


```
## spanning-tree bpdufilter 
### Description 
```
Configure interface specific bpdu-filter parameters.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree bpdufilter { enable | disable }
no spanning-tree bpdufilter
```
### Usage Guidelines 
```
These commands allow configuring interface specific bpdu-filter parameters
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree bpdufilter enable
sonic(conf-if-po1)# spanning-tree bpdufilter disable
```
## spanning-tree bpduguard 
### Description 
```
Configure interface specific bpdu-guard parameters.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree bpduguard [ port-shutdown ]
no spanning-tree bpduguard [ port-shutdown ]
```
### Usage Guidelines 
```
This commands allows enabling bpdu-guard on an interface
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree bpduguard port-shutdown
```
## spanning-tree cost 
### Description 
```
Configure spanning-tree cost on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree cost <value>
no spanning-tree cost
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |
### Usage Guidelines 
```
This command allows to configure the port level cost value, range 1 - 200000000
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree cost 1000
```
## spanning-tree edge-port 
### Description 
```
Configure spanning-tree global level BPDU filter
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree edge-port bpdufilter default
no spanning-tree edge-port bpdufilter default
```
### Usage Guidelines 
```
This command allows configuring global level BPDU filter
```
### Examples 
```
sonic(config)# spanning-tree edge-port bpdufilter default
```
## spanning-tree enable 
### Description 
```
Configure spanning-tree on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree enable
no spanning-tree enable
```
### Usage Guidelines 
```
This command allows enabling of spanning-tree on an interface
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree enable
```
## spanning-tree forward-time 
### Description 
```
Configure the spanning-tree forward delay time.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree forward-time <seconds>
no spanning-tree forward-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| seconds |   | Integer  |
### Usage Guidelines 
```
This command allows configuring the forward delay time in seconds (default = 15), range 4-30.
```
### Examples 
```
sonic(config)# spanning-tree forward-time 20
```
## spanning-tree guard 
### Description 
```
Configure the spanning-tree root guard timeout.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree guard root { timeout <value> }
no spanning-tree guard root timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value | timeout in seconds  | Integer  |
### Usage Guidelines 
```
This command allows configuring a root guard timeout value. Once superior BPDUs stop coming on the port, device will wait for a period until root guard timeout before moving the port to forwarding state(default = 30 secs), range 5-600.
```
### Examples 
```
sonic(config)# spanning-tree guard root timeout 10
```
## spanning-tree guard 
### Description 
```
Configure interface specific guard root parameters.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
spanning-tree guard root
no spanning-tree guard root
```
### Usage Guidelines 
```
This commands allows enabling guard root on an interface
```
### Examples 
```
sonic(config)# interface Ethernet 0
sonic(conf-if-Ethernet0)# spanning-tree guard root
```
## spanning-tree guard 
### Description 
```
Configure interface specific guard root parameters.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree guard root
no spanning-tree guard root
```
### Usage Guidelines 
```
This commands allows enabling guard root on an interface
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree guard root
```
## spanning-tree hello-time 
### Description 
```
Configure the spanning-tree hello time value.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree hello-time <seconds>
no spanning-tree hello-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| seconds |   | Integer  |
### Usage Guidelines 
```
This command allow configuring the hello interval in secs for transmission of bpdus (default = 2), range 1-10.
```
### Examples 
```
sonic(config)# spanning-tree hello-time 3
```
## spanning-tree link-type 
### Description 
```
Configure spanning-tree link-type on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree link-type { auto | point-to-point | shared }
no spanning-tree link-type
```
### Usage Guidelines 
```
This command allows setting the link-type of spanning-tree on an interface, link-type can be set to either point-point or shared.
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree link-type point-to-point
```
## spanning-tree max-age 
### Description 
```
Configure the spanning-tree max-age time value.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree max-age <seconds>
no spanning-tree max-age
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| seconds |   | Integer  |
### Usage Guidelines 
```
This command allows configuring the maximum time to listen for root bridge in seconds (default = 20), range 6-40.
```
### Examples 
```
sonic(config)# spanning-tree max-age 22
```
## spanning-tree mode 
### Description 
```
Configure the global spanning-tree mode for the device
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree mode { [ pvst ] | [ rapid-pvst ] }
no spanning-tree mode
```
### Usage Guidelines 
```
This command allows configuring the spanning-tree mode for the device. There are 2 modes supported - pvst and rapid-pvst.
```
### Examples 
```
sonic(config)#spanning-tree mode pvst
```
## spanning-tree port 
### Description 
```
Configure spanning-tree port type on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree port type edge
no spanning-tree port [ type ]
```
### Usage Guidelines 
```
This command allows setting edge-port type to an interface
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree port type edge
```
## spanning-tree port-priority 
### Description 
```
Configure spanning-tree port priority on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree port-priority <value>
no spanning-tree port-priority
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |
### Usage Guidelines 
```
This command allows setting port priority value on an interface, range 0 - 240 (default 128)
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree port-priority 16
```
## spanning-tree portfast 
### Description 
```
Configure spanning-tree portfast on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree portfast
no spanning-tree portfast
```
### Usage Guidelines 
```
This command allows enabling portfast on an interface, portfast allows edge ports to move to forwarding state quickly when the connected device is not participating in spanning-tree.
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree portfast
```
## spanning-tree priority 
### Description 
```
Configure the global level spanning-tree bridge priority value.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree priority <value>
no spanning-tree priority
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| value |   | Integer  |
### Usage Guidelines 
```
This command allows configuring the bridge priority in increments of 4096, range 0-61440
```
### Examples 
```
sonic(config)# spanning-tree priority 4096
```
## spanning-tree uplinkfast 
### Description 
```
Configure spanning-tree uplink fast on an interface.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree uplinkfast
no spanning-tree uplinkfast
```
### Usage Guidelines 
```
Uplink fast feature enhances STP performance for switches with redundant uplinks. Using the default value for the standard STP forward delay,
convergence following a transition from an active link to a redundant link can take 30 seconds (15 seconds for listening and an
additional 15 seconds for learning).
When uplink fast is configured on the redundant uplinks, it reduces the convergence time to just one second by moving to forwarding
state (bypassing listening and learning modes) in just once second when the active link goes down.
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree uplinkfast
```
## spanning-tree vlan 
### Description 
```
Configure spanning-tree parameters on per VLAN basis
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
spanning-tree vlan <vlan-range> { { [ forward-time ] <seconds> } | { [ hello-time ] <seconds> } | { [ max-age ] <seconds> } | { [ priority ] <value> } }
no spanning-tree vlan <vlan-range> { [ forward-time ] | [ hello-time ] | [ max-age ] | [ priority ] }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-range | VLAN ID  | Integer  |
| seconds |   | Integer  |
| value |   | Integer  |
### Usage Guidelines 
```
These commands are similar to the global level commands but allow configuring the spanning-tree parameters on per VLAN basis.
```
### Examples 
```
sonic(config)#spanning-tree vlan 100
sonic(config)#spanning-tree vlan 100 forward-time 11
sonic(config)#spanning-tree vlan 100 hello-time 3
sonic(config)#spanning-tree vlan 100 max-age 22
sonic(config)#spanning-tree vlan 100 priority 4096
```
## spanning-tree vlan 
### Description 
```
Configure interface and vlan specific spanning-tree parameters.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
spanning-tree vlan <vlan-range> { { cost <value> } | { port-priority <value> } }
no spanning-tree vlan <vlan-range> { cost | port-priority }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-range | VLAN ID  | Integer  |
| value |   | Integer  |
### Usage Guidelines 
```
This commands allows configuring interface and vlan specific spanning-tree parameters.
```
### Examples 
```
sonic(config)# interface Ethernet 0
sonic(conf-if-Ethernet0)# spanning-tree vlan 100 cost 1000
sonic(conf-if-Ethernet0)# spanning-tree vlan 100 port-priority 16
```
## spanning-tree vlan 
### Description 
```
Configure interface and vlan specific spanning-tree parameters.
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
spanning-tree vlan <vlan-range> { { cost <value> } | { port-priority <value> } }
no spanning-tree vlan <vlan-range> { cost | port-priority }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-range | VLAN ID  | Integer  |
| value |   | Integer  |
### Usage Guidelines 
```
This commands allows configuring interface and vlan specific spanning-tree parameters.
```
### Examples 
```
sonic(config)# interface PortChannel 1
sonic(conf-if-po1)# spanning-tree vlan 100 cost 1000
sonic(conf-if-po1)# spanning-tree vlan 100 port-priority 16
```
## speed 
### Description 
```
Configure speed 
```
### Parent Commands (Modes) 
```
interface Management <mgmt-if-id>
```
### Syntax 
```
speed <speed>
no speed
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| speed | Port speed  | Select [10(10MBPS) 100(100MBPS) 1000(1GIGE) auto(1GIGE) ]  |
## static 
### Description 
```
Add static NAT entry 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
static { { basic <global-ip> <local-ip> [ <natType> ] { [ twice-nat-id ] <twice-nat-id-value> } } | { <natPortType> <global-ip> <global-port> <local-ip> <local-port> [ <natType> ] { [ twice-nat-id ] <twice-nat-id-value> } } }
no static { all | { basic <global-ip> } | { <natPortType> <global-ip> <global-port> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| global-ip | A.B.C.D  | String  |
| local-ip | A.B.C.D  | String  |
| natType | NAT type  | Select [snat dnat ]  |
| twice-nat-id-value | Unsigned integer  | String  |
| natPortType | NAT Port type  | Select [tcp udp ]  |
| global-port | Unsigned integer  | String  |
| local-port | Unsigned integer  | String  |
## strict-capability-match 
### Description 
```
This command instructs BGP to strictly compare remote capabilities and
local capabilities. If capabilities are different, send Unsupported
Capability error then reset connection.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
strict-capability-match
no strict-capability-match
```
### Usage Guidelines 
```
Use this command for a BGP neighbor to enforce exact matching of sent
and received capabilities
```
### Examples 
#### Following command enables strict capability match           for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# strict-capability-match
```
## strict-capability-match 
### Description 
```
This command instructs BGP to strictly compare remote capabilities and
local capabilities. If capabilities are different, send Unsupported
Capability error then reset connection.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
strict-capability-match
no strict-capability-match
```
### Usage Guidelines 
```
Use this command for a BGP peer-group to enforce exact matching of sent
and received capabilities
```
### Examples 
#### Following command enables strict capability match           for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# strict-capability-match
```
## switchport access 
### Description 
```
Set access mode characteristics of the interface 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
switchport access Vlan <vlan-id>
no switchport access Vlan
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id |   | Integer  |
## switchport access 
### Description 
```
Set access mode characteristics of the interface 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
switchport access Vlan <vlan-id>
no switchport access Vlan
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan-id |   | Integer  |
## switchport trunk 
### Description 
```
Configure trunking parameters on an interface 
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
switchport trunk allowed { Vlan <vlan_id_list> }
no switchport trunk allowed { Vlan <vlan_id_list> }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan_id_list |   | String  |
## switchport trunk 
### Description 
```
Configure trunking parameters on an interface 
```
### Parent Commands (Modes) 
```
interface PortChannel <lag-id> [ mode ] <PoMode> [ min-links ] <min-links-value> [ fallback ]
```
### Syntax 
```
switchport trunk allowed { Vlan <vlan_id_list> }
no switchport trunk allowed { Vlan <vlan_id_list> }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vlan_id_list |   | String  |
## table-map 
### Description 
```
This command enables user to apply a route-map on route updates from BGP
to Zebra
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
table-map <rtmap>
no table-map [ <rtmap> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtmap | String  | String  |
### Usage Guidelines 
```
This command enables user to apply a route-map on route updates from BGP to
Zebra (RIB manager). All the applicable match operations are allowed, such as match on
prefix, next-hop, communities, etc. Set operations for this attach-point
are limited to metric and next-hop only. Any operation of this feature
does not affect BGPs internal RIB.
```
### Examples 
#### Following example configures a table-map rmap_block_private 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# address-family ipv4 unicast
sonic(config-router-bgp-af)# table-map rmap_block_private
```
## table-map 
### Description 
```
BGP table to RIB route download filter 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
table-map <rtmap>
no table-map [ <rtmap> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| rtmap | String  | String  |
## tacacs-server auth-type 
### Description 
```
Configure global authentication type for TACACS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
tacacs-server auth-type <auth-type>
no tacacs-server auth-type
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| auth-type |   | Select [pap(pap) chap(chap) mschap(mschap) ]  |
## tacacs-server host 
### Description 
```
Configure a server for TACACS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
tacacs-server host <host> [ port ] <port-val> [ timeout ] <timeout-val> [ key ] <key-val> [ type ] <type-val> [ priority ] <priority-val>
no tacacs-server host <address>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| host | A.B.C.D/A::B  | String  |
| port-val | port  | Integer  |
| timeout-val | seconds  | Integer  |
| key-val | (Valid Chars: ASCII printable except SPACE, #, and COMMA, Max Len: 65) shared secret  | String  |
| type-val |   | Select [pap(pap) chap(chap) mschap(mschap) ]  |
| priority-val | (1..64)  | Integer  |
## tacacs-server key 
### Description 
```
Configure global shared secret for TACACS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
tacacs-server key <secret-key>
no tacacs-server key
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| secret-key | (Valid Chars: ASCII printable except SPACE, #, and COMMA, Max Len: 65) shared secret  | String  |
## tacacs-server source-ip 
### Description 
```
Configure global source ip for TACACS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
tacacs-server source-ip <src-ip>
no tacacs-server source-ip
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| src-ip | A.B.C.D/A::B  | String  |
## tacacs-server timeout 
### Description 
```
Configure global timeout for TACACS 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
tacacs-server timeout <timeout>
no tacacs-server timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| timeout | seconds  | Integer  |
## tam 

### Description 

```
TAM Device Configuration 


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
tam

```
## tcp-timeout 
### Description 
```
Configure TCP NAT entry aging timeout in seconds 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
tcp-timeout <tcp-timeout-value>
no tcp-timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| tcp-timeout-value |   | Integer  |
## terminal length 

### Description 

```
Set terminal length 


```
### Syntax 

```
terminal length <length>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| length |   | Integer  |


## timeout 
### Description 
```
Timeout value (1-999) 
```
### Parent Commands (Modes) 
```
link state track <grp-name>
```
### Syntax 
```
timeout <grp-tmout>
no timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| grp-tmout | Unsigned integer  | String  |
## timeout 
### Description 
```
Configure NAT entry aging timeout in seconds 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
timeout <timeout-value>
no timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| timeout-value |   | Integer  |
## timers 
### Description 
```
This command configures keelapive and hold timer interval (in seconds)
at a global level.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
timers <keepalive-intvl> <hold-time>
no timers <keepalive-intvl> <hold-time>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| keepalive-intvl |   | Integer  |
| hold-time |   | Integer  |
### Usage Guidelines 
```
Use this command to configure keepalive and hold timer interval for an
instnace of BGP. Note that keepalive timer interval must be smaller than
hold timer interval.
```
### Examples 
#### Below command configures Keepalive interval to 10sec and          hold timer interval to 30sec 
```
         sonic# configure terminal
         sonic(config)# router bgp 65300
         sonic(config-router-bgp)# timers 10 30
```
## timers 
### Description 
```
This command enables user to configure keepalive, hold and connect timer
intervals for a BGP neighbor.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
timers { { <keepalive-intvl> <hold-time> } | { connect <connect-time> } }
no timers { { <keepalive-intvl> <hold-time> } | { connect <connect-time> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| keepalive-intvl |   | Integer  |
| hold-time |   | Integer  |
| connect-time |   | Integer  |
### Usage Guidelines 
```
Use this command to configure keeplaive, hold and connect retry timer
intervals for a BGP neighbor.
```
### Examples 
#### Following command configures keepalive and hold timer          interval for neighbor 30.30.30.3 to 3 and 9 seconds respectively 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# timers 3 9
```
## timers 
### Description 
```
This command enables user to configure keepalive, hold and connect timer
intervals for a BGP peer-group.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
timers { { <keepalive-intvl> <hold-time> } | { connect <connect-time> } }
no timers { { <keepalive-intvl> <hold-time> } | { connect <connect-time> } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| keepalive-intvl |   | Integer  |
| hold-time |   | Integer  |
| connect-time |   | Integer  |
### Usage Guidelines 
```
Use this command to configure keeplaive, hold and connect retry timer
intervals for a BGP peer-group.
```
### Examples 
#### Following command configures keepalive and hold timer          interval for peer-group PG_Ext to 3 and 9 seconds respectively 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# timers 3 9
```
## transmit-interval 

### Description 

```
Configure desired packet transmit interval for Bidirectional Forwarding detection(BFD) peer.


```
### Parent Commands (Modes) 

```
peer <peer_ipv4>
peer <peer_ipv6>
peer [ interface ] <interfacename>
peer [ local-address ] <local_ipv4>
peer [ local-address ] <local_ipv6>
peer [ multihop ]
peer [ vrf ] <vrfname>

```
### Syntax 

```
transmit-interval <transmit_interval>

```
### Parameters 

| Name | Description | Type |
|:---:|:-----:|:-----:|
| transmit_interval |   | Integer  |


### Usage Guidelines 

```
Default value is 300 milliseconds.


```
### Examples 
#### Configure packet transmit interval 

```
device()#configure terminal
device(config)#bfd
device(conf-bfd)# peer 192.168.0.5 interface Ethernet0
device(conf-bfd-peer)# transmit-interval 200


```
## ttl-security hops 
### Description 
```
This command enforces Generalized TTL Security Mechanism (GTSM), as
specified in RFC 5082. With this command, only neighbors that are the
specified number of hops away will be allowed to become neighbors. This
command is mutually exclusive with ebgp-multihop.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
ttl-security hops <nhops>
no ttl-security hops
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| nhops |   | Integer  |
### Usage Guidelines 
```
Use this command for a BGP neighbor to enable Generalized TTL Security
Mechanism (GTSM). This is for security purposes.
```
### Examples 
#### Following command enables GTSM for BGP neighbor 30.30.30.3 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# ttl-security hops 6
```
## ttl-security hops 
### Description 
```
This command enforces Generalized TTL Security Mechanism (GTSM), as
specified in RFC 5082. With this command, only neighbors that are the
specified number of hops away will be allowed to become neighbors. This
command is mutually exclusive with ebgp-multihop.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
ttl-security hops <nhops>
no ttl-security hops
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| nhops |   | Integer  |
### Usage Guidelines 
```
Use this command for a BGP peer-group to enable Generalized TTL Security
Mechanism (GTSM). This is for security purposes.
```
### Examples 
#### Following command enables GTSM for BGP peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# ttl-security hops 8
```
## udld aggressive 
### Description 
```
Configure UDLD mode to aggressive.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
udld aggressive
no udld aggressive
```
### Usage Guidelines 
```
Use this command to change UDLD mode to aggressive. Default UDLD mode is normal.
```
### Examples 
#### Configure UDLD mode to aggressive 
```
sonic-cli(config)# udld enable
sonic-cli(config)# udld aggressive
```
## udld aggressive 
### Description 
```
Enable aggressive mode of UDLD at interface level.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
udld aggressive
no udld aggressive
```
### Usage Guidelines 
```
Use this command to change UDLD mode to aggressive at interface level. Default UDLD mode is normal.
```
### Examples 
#### Enable aggressive mode of UDLD at interface level 
```
sonic-cli(config)# interface Ethernet 0
sonic-cli(conf-if-Ethernet0)# udld enable
sonic-cli(conf-if-Ethernet0)# udld aggressive
```
## udld enable 
### Description 
```
Enable UDLD at global level
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
udld enable
no udld enable
```
### Usage Guidelines 
```
Use this command to enable UDLD globally
```
### Examples 
#### Enable UDLD at global level 
```
sonic-cli(config)# udld enable
```
## udld enable 
### Description 
```
Enable UDLD at interface level.
```
### Parent Commands (Modes) 
```
interface <phy-if-name>
```
### Syntax 
```
udld enable
no udld enable
```
### Usage Guidelines 
```
Use this command to enable UDLD at interface level
```
### Examples 
#### Enable UDLD at interface level 
```
sonic-cli(config)# interface Ethernet 0
sonic-cli(conf-if-Ethernet0)# udld enable
```
## udld message-time 
### Description 
```
Configure UDLD message time. It is the time interval at which periodic hellos are exchanged.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
udld message-time <msg-time>
no udld message-time
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| msg-time |   | Integer  |
### Usage Guidelines 
```
Use this command to set UDLD message time. Default message time is 1 second.
```
### Examples 
#### Configure UDLD message time 
```
sonic-cli(config)# udld enable
sonic-cli(config)# udld message-time 3
```
## udld multiplier 
### Description 
```
Configure UDLD multiplier value. This multiplier value is used to determine the timeout interval (i.e. message-time x multiplier value) after which UDLD declares the link as Unidirectonal.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
udld multiplier <multiplier>
no udld multiplier
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| multiplier |   | Integer  |
### Usage Guidelines 
```
Use this command to set UDLD multiplier value. Default multiplier value is 3.
```
### Examples 
#### Configure UDLD multiplier value 
```
sonic-cli(config)# udld enable
sonic-cli(config)# udld multiplier 8
```
## udp-timeout 
### Description 
```
Configure UDP NAT entry aging timeout in seconds 
```
### Parent Commands (Modes) 
```
nat
```
### Syntax 
```
udp-timeout <udp-timeout-value>
no udp-timeout
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| udp-timeout-value |   | Integer  |
## unsuppress-map 
### Description 
```
This command configures a Route-map to selectively unsuppress
suppressed routes
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
### Usage Guidelines 
```
Use this command to define a route policy via route-map to unsuppress
suppressed routes.
```
### Examples 
#### Following command configures an unsuppress map for neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# unsuppress-map rm_unsup_ext_rt
```
## unsuppress-map 
### Description 
```
This command configures a Route-map to selectively unsuppress
suppressed routes
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
### Usage Guidelines 
```
Use this command to define a route policy via route-map to unsuppress
suppressed routes.
```
### Examples 
#### Following command configures an unsuppress map for a          peer-group 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# unsuppress-map rm_unsup_ext_rt
```
## unsuppress-map 
### Description 
```
Route-map to selectively unsuppress suppressed routes 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
## unsuppress-map 
### Description 
```
Route-map to selectively unsuppress suppressed routes 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
## unsuppress-map 
### Description 
```
Route-map to selectively unsuppress suppressed routes 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
## unsuppress-map 
### Description 
```
Route-map to selectively unsuppress suppressed routes 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
unsuppress-map <map>
no unsuppress-map <map>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| map | String  | String  |
## update-delay 
### Description 
```
This command allows user to set update delay. This parameter control how
long to wait before running best-path selection after Graceful Restart.
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
update-delay <time> [ <maxmedval> ]
no update-delay
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| time |   | Integer  |
| maxmedval |   | Integer  |
### Usage Guidelines 
```
This feature is used to enable read-only mode on BGP process restart or
when BGP process is cleared using clear ip bgp *. When applicable,
read-only mode would begin as soon as the first peer reaches Established
status and a timer for max-delay seconds is started.
During this mode BGP doesn't run any best-path or generate any updates
to its peers. This mode continues until:
All the configured peers, except the shutdown peers, have sent explicit
EOR (End-Of-RIB) or an implicit-EOR. The first keep-alive after BGP has
reached Established is considered an implicit-EOR. If the establish-wait
optional value is given, then BGP will wait for peers to reach
established from the beginning of the update-delay till the
establish-wait period is over, i.e. the minimum set of established peers
for which EOR is expected would be peers established during the
establish-wait window, not necessarily all the configured neighbors.
max-delay period is over.
On hitting any of the above two conditions, BGP resumes the decision
process and generates updates to its peers.
Default max-delay is 0, i.e. the feature is off by default.
```
### Examples 
#### Below command configures update-delay to 120 seconds 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# update-delay 120
```
## update-source 
### Description 
```
This command specifies the IPv4 or IPv6 source address to use for the
BGP session to this neighbor. Source address may be specified as either
an IPv4/IPv6 address directly or as an interface name. The interface
name could be router port or Port Channel or Vlan interface with
IPv4/IPv6 address configured on it.
```
### Parent Commands (Modes) 
```
neighbor { <ip> | { interface { Ethernet | PortChannel | Vlan } } }
```
### Syntax 
```
update-source { <ip> | { interface { Ethernet | PortChannel | Vlan | Loopback } } }
no update-source { [ <ip> ] | { interface { Ethernet | PortChannel | Vlan | Loopback } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip | A.B.C.D/A::B  | String  |
### Usage Guidelines 
```
Use this command to configure source interface for a BGP neighbor
sessions
```
### Examples 
#### Following command configures source interface           for neighbor 30.30.30.3 to 12.56.36.74 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 30.30.30.3
sonic(config-router-bgp-neighbor)# update-source 12.56.36.74
```
## update-source 
### Description 
```
This command specifies the IPv4 or IPv6 source address to use for the
BGP session to neighbors in a peer-group. Source address may be specified
as either an IPv4/IPv6 address directly or as an interface name. The
interface name could be router port or Port Channel or Vlan interface with
IPv4/IPv6 address configured on it.
```
### Parent Commands (Modes) 
```
peer-group <template-str>
```
### Syntax 
```
update-source { <ip> | { interface { Ethernet | PortChannel | Vlan | Loopback } } }
no update-source { [ <ip> ] | { interface { Ethernet | PortChannel | Vlan | Loopback } } }
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| ip | A.B.C.D/A::B  | String  |
### Usage Guidelines 
```
Use this command to configure source interface for a BGP peer-group
```
### Examples 
#### Following command configures source interface           for peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Ext
sonic(config-router-bgp-pg)# update-source Ethernet16
```
## username 
### Description 
```
Add new user 
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
username <user-name> password { <passwd> { role <rl> } }
no username <user-name>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| user-name | String  | String  |
| passwd | String  | String  |
| rl | String  | String  |
## vni 
### Description 
```
Enter VNI config mode 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
vni <vninum>
no vni <vninum>
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| vninum | VNI  | Integer  |
## weight 
### Description 
```
This command configures a default weight for all routes received from
this BGP neighbor
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
### Usage Guidelines 
```
Use this command to assign a default weight to BGP routes received from
this neighbor. Weight parameter is used in BGP route selection process.
So, configuring weight may influence the outcome of the route selection
process
```
### Examples 
#### Following command configures a default weight of 45 for          routes received from neighbor 20.20.20.2 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# neighbor 20.20.20.2
sonic(config-router-bgp-neighbor)# remote-as 300
sonic(config-router-bgp-neighbor)# address-family ipv4 unicast
sonic(config-router-bgp-neighbor-af)# weight 45
```
## weight 
### Description 
```
This command configures a default weight for all routes received from
neighbors in this peer-group
```
### Parent Commands (Modes) 
```
address-family ipv4 unicast
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
### Usage Guidelines 
```
Use this command to assign a default weight to BGP routes received from
neighbors in this peer-group. Weight parameter is used in BGP route
selection process.  So, configuring weight may influence the outcome of
the route selection process
```
### Examples 
#### Following command configures a default weight of 25 for          routes received from neighbors in peer-group PG_Ext 
```
sonic# configure terminal
sonic(config)# router bgp 100
sonic(config-router-bgp)# peer-group PG_Int
sonic(config-router-bgp-pg)# address-family ipv4 unicast
sonic(config-router-bgp-pg-af)# weight 25
```
## weight 
### Description 
```
Set default weight for routes from this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
## weight 
### Description 
```
Set default weight for routes from this neighbor 
```
### Parent Commands (Modes) 
```
address-family ipv6 unicast
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
## weight 
### Description 
```
Set default weight for routes from this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
## weight 
### Description 
```
Set default weight for routes from this neighbor 
```
### Parent Commands (Modes) 
```
address-family l2vpn evpn
```
### Syntax 
```
weight <val>
no weight [ <val> ]
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| val |   | Integer  |
## write 

### Description 

```
Save config 


```
### Syntax 

```
write memory

```
## write erase 
### Description 
```
Erase the existing switch configuration files except the management interface configuration,
or cancel the configuration erase operation.
"write erase" command deletes the startup configuration JSON file and all application
configuration files in the /etc/sonic directory. The management interface configuration
in the startup configuration file is retained so that the user can access the switch using
the same management address after the switch reboot.
For the write erase command operation to take effect, the user has to reboot the switch
after issuing the write erase command. If the user wishes to not proceed with the configuration
removal operation, the write erase cancel command can be used to undo the previously issued
write erase command.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
write erase
no write erase
```
### Usage Guidelines 
```
Use the command "write erase" to erase the existing switch configuration files except for the management interface configuration.
Use the command "no write erase" to cancel configuration erase operation.
```
### Examples 
```
sonic# configure terminal
sonic(config)# write erase
Existing switch configuration files except management interface configuration will be removed, continue? [y/N]:
sonic(config)# no write erase
Switch configuration erase operation will be cancelled, continue? [y/N]:
```
## write erase boot 

### Description 

```
Erase the configuration files including management interface configuration.

The "write erase boot" command deletes the startup configuration JSON file and all
application configuration files in the /etc/sonic directory. The management
interface configuration in the startup configuration JSON file is also removed.
The SONiC switch boots with a factory default configuration file.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
write erase boot

```
### Usage Guidelines 

```
Use this command to erase the configuration files including the management
interface configuration.


```
### Examples 

```
sonic# configure terminal
sonic(config)# write erase boot
Existing switch configuration files will be removed, continue? [y/N]:


```
## write erase install 

### Description 

```
Restore SONiC switch content to default values.

The "write erase install" command removes all changes made by the user.
All user installed packages and file changes are removed. It also deletes
the startup configuration JSON file and the files in /etc/sonic directory.
The SONiC switch is reverted to the same state as a newly installed image.
After the SONiC switch is rebooted, if the Zero Touch Provisioning (ZTP)
feature is enabled, the SONIC switch will start performing ZTP to discover
and download the switch configuration.


```
### Parent Commands (Modes) 

```
configure terminal

```
### Syntax 

```
write erase install

```
### Usage Guidelines 

```
Use this command to restore SONiC switch content to default values.


```
### Examples 

```
sonic# configure terminal
sonic(config)# write erase install
All SONiC switch content will be restored to default values, continue? [y/N]:


```
## write-quanta 
### Description 
```
This command configures the maximum number of BGP packets to write to
peer socker in one cycle of I/O
```
### Parent Commands (Modes) 
```
router bgp { <as-num-dot> { [ vrf ] <vrf-name> } }
```
### Syntax 
```
write-quanta <wrval>
no write-quanta
```
### Parameters 
| Name | Description | Type |
|:---:|:-----:|:-----:|
| wrval |   | Integer  |
### Usage Guidelines 
```
BGP message Tx I/O is vectored. This means that multiple packets are
written to the peer socket at the same time each I/O cycle, in order to
minimize system call overhead. This value controls how many are written
at a time. Under certain load conditions, reducing this value could make
peer traffic less bursty. In practice, leave this settings on the
default (64).
```
### Examples 
#### Below command configures the write-quanta to          50 packets 
```
sonic# configure terminal
sonic(config)# router bgp 65300
sonic(config-router-bgp)# write-quanta 50
```
## ztp enable 
### Description 
```
Administratively enable or disable ZTP.
```
### Parent Commands (Modes) 
```
configure terminal
```
### Syntax 
```
ztp enable
no ztp enable
```
### Usage Guidelines 
```
Use these commands to administratively enable or disable ZTP.
```
### Examples 
```
sonic# configure terminal
sonic(config)# ztp enable
sonic(config)# no ztp enable
```
