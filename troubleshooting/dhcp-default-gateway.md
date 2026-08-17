```markdown
# DHCP Client Missing Default Gateway

## Problem

The Windows client received an IP address from DHCP but did not receive a default gateway.

## Environment

- Windows Server 2022
- Windows client
- Active Directory
- DHCP
- DNS
- Routing and NAT
- VirtualBox internal network

## Symptoms

The Windows client successfully received an IP address.

However, the client did not have a default gateway.

## Investigation

I checked the client's network configuration using:

powershell
ipconfig
