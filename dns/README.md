
The transcript describes the two-interface design and the Domain Controller's role in routing internal client traffic. :contentReference[oaicite:1]{index=1}

---

# 4. `dns/README.md`

```markdown
# DNS Configuration

## Objective

The objective of this section was to configure DNS for the Active Directory domain and allow domain clients to resolve the Domain Controller and domain resources.

## DNS and Active Directory

DNS is used by Active Directory to locate domain services.

The Domain Controller also serves as the DNS server for the internal lab network.

## DNS Configuration

DNS was installed as part of the Active Directory Domain Services deployment.

The Windows client was configured to use the Domain Controller as its DNS server.

## Client Configuration

The DHCP server provides the Domain Controller's IP address as the DNS server for clients.

This allows the client to resolve the Active Directory domain.

## Verification

DNS configuration was verified using:

```powershell
ipconfig /all
