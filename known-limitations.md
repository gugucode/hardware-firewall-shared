---

copyright:
  years: 2017
lastupdated: "2018-11-12"

keywords: limitations, firewall, gateway, fortigate, fsa, subnet, vlan, problems, issues

subcollection: hardware-firewall-shared

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
{:codeblock: .codeblock}
{:pre: .pre}
{:screen: .screen}
{:tip: .tip}
{:note: .note}
{:important: .important}
{:download: .download}

# Known Limitations with Hardware Firewall
{: #known-limitations-with-hardware-firewall-shared-}

A Hardware Firewall cannot be deployed to a server on a VLAN that meets any of the following criteria.

* Is currently associated with a Network Gateway, Hardware Firewall, or FortiGate Security Appliance.
* Contains 30 or more servers.
* Has a primary subnet that is larger than a /28.

In these instances, a new VLAN must be established for the Firewall or another product must be selected.

Further limitations for the Hardware Firewall include:

* Portable subnets are not protected
* Not available for 10Gb servers
* Maximum of 79 firewall rules per Hardware Firewall
* Incompatible with Windows Network Load Balancing (NLB) due to the way ARP is processed
* The rule destination subnet is limited to the public IP of the protected server. Hardware Firewall (Dedicated) does not have this limitation.
* Hourly billed servers are not allowed. Hardware Firewall can be applied to a monthly billed server.
