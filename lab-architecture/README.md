# Lab Architecture

## Overview

This Active Directory lab uses virtual machines to simulate a small Windows enterprise network.

The environment consists of a Windows Server 2022 Domain Controller and a Windows client. The Domain Controller provides Active Directory Domain Services, DNS, DHCP, and routing/NAT services.

The client connects to an isolated internal network and uses the Domain Controller for network configuration, DNS resolution, domain authentication, and internet access.

## Lab Components

| Component | Role |
|---|---|
| Windows Server 2022 | Domain Controller |
| Windows 10/11 Client | Domain-joined workstation |
| Active Directory Domain Services | Centralized authentication and administration |
| DNS | Domain name resolution |
| DHCP | Automatic IP configuration |
| Routing and NAT | Internet access for internal clients |
| VirtualBox | Virtualization platform |
| PowerShell | Active Directory automation |

## Network Design

The Domain Controller uses two network interfaces.

The external interface provides internet connectivity.

The internal interface connects the Domain Controller to the private lab network.

The Domain Controller routes traffic from the internal network to the internet using NAT.

```text
                         Internet
                            |
                            |
                    External NIC
                            |
                  Windows Server 2022
                   Domain Controller
                    /      |       \
                   /       |        \
                AD DS     DNS      DHCP
                   |
              Routing / NAT
                   |
              Internal NIC
                   |
            Private Lab Network
                   |
                Client 1
             Windows 10/11
                   |
              Domain Join
