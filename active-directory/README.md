
---

# 2. `active-directory/README.md`

```markdown
# Active Directory

## Objective

The objective of this section was to deploy Active Directory Domain Services on Windows Server 2022 and establish a Windows domain for centralized authentication and administration.

## Environment

- Operating System: Windows Server 2022
- Role: Domain Controller
- Virtualization: VirtualBox
- Active Directory Domain Services: Installed
- DNS: Integrated with Active Directory

## Domain Controller

The Windows Server 2022 virtual machine was configured as the Domain Controller for the lab.

The server was renamed and configured before Active Directory Domain Services was installed.

## Active Directory Domain Services

Active Directory Domain Services was installed through Server Manager.

The server was then promoted to a Domain Controller by creating a new Active Directory forest and domain.

## Domain Structure

The domain contains organizational units used to organize administrative accounts and standard users.

```text
Domain
│
├── Admin OU
│
└── Users OU
