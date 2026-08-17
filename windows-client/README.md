Explains my script's name processing, OU creation, loop, username generation, and secure password handling.
---

# 9. `windows-client/README.md`

```markdown
# Windows Client

## Objective

The objective of this section was to deploy a Windows client, connect it to the internal lab network, obtain network configuration through DHCP, and join the Active Directory domain.

## Client Environment

- Operating System: Windows 10/11
- Role: Domain-joined workstation
- Network: Internal lab network
- Configuration: DHCP

## Network Configuration

The Windows client obtains its network configuration from the DHCP server running on the Domain Controller.

The client receives:

- IP address
- Subnet mask
- Default gateway
- DNS server

## Connectivity Testing

The client's network configuration was checked using:

powershell
ipconfig /all
