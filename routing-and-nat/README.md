
The transcript provides the DHCP scope and explains the gateway and DNS options. :contentReference[oaicite:3]{index=3}

---
# 6. `routing-and-nat/README.md`

```markdown
# Routing and NAT

## Objective

The objective of this section was to allow the private Windows client network to access the internet through the Domain Controller.

## Network Design

The Domain Controller has:

- An external network interface
- An internal network interface

The internal interface connects to the private lab network.

The external interface provides internet connectivity.

## Routing

Routing was configured on the Domain Controller so traffic from the internal client network could be forwarded toward the internet.

## NAT

Network Address Translation was configured so internal clients could access the internet through the Domain Controller's external connection.

```text
Windows Client
      |
Internal Network
      |
Domain Controller
      |
NAT
      |
Internet
