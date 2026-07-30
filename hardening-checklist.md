# Hardening Checklist

## v1 - Basic Lynis Suggestions

### 1. UFW Firewall (Uncomplicated FireWall)
- Action: Installed and enabled UFW, allowed SSH
- Status: Complete

### 2. SSH Hardening
- Action: Disabled root login, set MaxAuthTries to 4
- Status: Complete

### 3. Fail2ban
- Action: Installed, enabled, and started Fail2ban
- Status: Complete

## v2 - Lynis Suggestion Remediation (July 2026)

Baseline: lynis-current.txt, 1 warning / 38 suggestions

| # | Finding                      | Severity   | Status      | Fix Applied | Index After | 
|---|------------------------------|------------|-------------|-------------|-------------|
| 1 | /etc/sudoers.d permissions   | Warning    | Not Started |             |             |
| 2 | Vulnerable packages present  | Warning    | Not Started |             |             |
| 3 | sshd_config suggestions      | Suggestion | Not Started |             |             |
| 4 | PAM password strength        | Suggestion | Not Started |             |             |
| 5 | Password hashing methods     | Suggestion | Not Started |             |             |
| 6 | Accounts without expire date | Suggestion | Not Started |             |             |
| | |

