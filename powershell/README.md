
---

# 8. `powershell/README.md`

```markdown
# PowerShell Active Directory Automation

## Objective

The objective of this section was to automate Active Directory user creation using PowerShell.

Manually creating a large number of user accounts would take significant time, so PowerShell was used to automate the process.

## Automation Process

The PowerShell script uses a list of names as input.

The script then processes each name and creates an Active Directory user account.

The general process is:

```text
Names File
    |
    v
PowerShell Script
    |
    v
Process Names
    |
    v
Generate Usernames
    |
    v
Create Users OU
    |
    v
Create Active Directory Users
