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

Baseline: lynis-current.txt, 2 warning / 38 suggestions (Highest Yield Fixes)

| # | Finding                      | Severity   | Status      | Fix Applied                                                     | Index After                  | 
|---|------------------------------|------------|-------------|-----------------------------------------------------------------|------------------------------|
| 1 | /etc/sudoers.d permissions   | Warning    | Resolved    | Patched 'Others' access (regular users can't access sudoers dir |                              |
| 2 | Vulnerable packages present  | Warning    | Resolved    | Patched to current, no security packages left                   | 67 (fixed 1 & 2)             |
| 3 | sshd_config suggestions      | Suggestion | Resolved    | Patched so no one can view except root (not group or others)    | 67 (confirmed w test status) |
| 4 | PAM password strength        | Suggestion | Resolved    | Installed Libpasswdqc files + update (went down, came up aftr)  | 66 (confirmed via test still down 1)
)                             |


