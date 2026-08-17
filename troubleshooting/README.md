
Shows the client receiving its IP configuration, troubleshooting the gateway, testing internet connectivity, renaming the computer, and joining the domain.

---

# 10. `troubleshooting/README.md`

```markdown
# Troubleshooting

## Overview

This section documents technical problems encountered while building and testing the Active Directory lab.

Each troubleshooting entry documents:

1. Problem
2. Symptoms
3. Investigation
4. Root Cause
5. Solution
6. Verification
7. Lessons Learned

## Troubleshooting Cases

### DHCP Default Gateway

The Windows client received an IP address but did not receive a default gateway.

[View Troubleshooting Report](dhcp-default-gateway.md)

## Troubleshooting Methodology

When troubleshooting the lab, I follow a structured process:

```text
Identify Problem
      |
      v
Collect Information
      |
      v
Test Connectivity
      |
      v
Check Configuration
      |
      v
Identify Root Cause
      |
      v
Apply Fix
      |
      v
Verify Solution
      |
      v
Document Results
