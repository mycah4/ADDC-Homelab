Explains using the Domain Controller as DNS because Active Directory installs DNS and the client needs the DC as its DNS server. :contentReference[oaicite:2]{index=2}

---

# 5. `dhcp/README.md`

```markdown
# DHCP Configuration

## Objective

The objective of this section was to configure DHCP so Windows clients automatically receive the network information required to communicate with the lab network, Domain Controller, and internet.

## DHCP Server

The DHCP role was installed on the Windows Server 2022 Domain Controller.

The DHCP server provides clients with network configuration automatically.

## DHCP Scope

The lab uses a DHCP scope for the internal network.

Example configuration:

| Setting | Value |
|---|---|
| Network | 172.16.0.0/24 |
| Start Address | 172.16.0.100 |
| End Address | 172.16.0.200 |
| Subnet Mask | 255.255.255.0 |

The exact values were adjusted based on the lab configuration.

## DHCP Options

The DHCP server provides clients with:

- IP address
- Subnet mask
- Default gateway
- DNS server

The Domain Controller's internal IP address is used for the default gateway and DNS server.

## DHCP Authorization

The DHCP server was authorized and the DHCP scope was activated.

## Client Lease

The Windows client obtains its IP configuration automatically from the DHCP server.

## Verification

The client configuration was checked using:

powershell
ipconfig /all
