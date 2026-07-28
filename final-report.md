# Final Report: Home Server Security Assessment

## Summary
Baseline security assessment performed on a Linux home server VM.
Identified risks, applied hardening steps, and verified improvements.

## Before
- Hardening Index: 63
- Firewall: Active
- Intrusion software: not detected
- SSH: default settings, root login enabled (problem bc it's the highest auth)

## Hardening Applied
- Enabled UFW (Uncomplicated FireWall)
- Disabled root login over SSH
- Enabled and set MaxAuthTries to 4
- Installed and enabled Fail2ban

## After
- Hardening Index: 61
- Firewall: Active
- Intrusion software: detected
- SSH: root login disabled, auth attempts limited to 4 and enforced by Fail2ban

## Conclusion
Three medium findings resolved. System exposure reduced.
Project demonstrates baseline defensive security workflow.
