
The transcript supports the domain creation, administrative OU, dedicated administrator, and Domain Admins configuration.

---

# 3. `networking/README.md`

```markdown
# Network Configuration

## Objective

The objective of this section was to create an isolated network for the Active Directory lab while allowing the Windows client to access the internet through the Domain Controller.

## Network Interfaces

The Domain Controller uses two network interfaces.

### External Interface

The external interface connects the Domain Controller to the internet.

### Internal Interface

The internal interface connects the Domain Controller to the private lab network.

The Windows client connects to this internal network.

## Network Architecture


Internet
   |
External NIC
   |
Domain Controller
   |
Internal NIC
   |
Private Network
   |
Windows Client
