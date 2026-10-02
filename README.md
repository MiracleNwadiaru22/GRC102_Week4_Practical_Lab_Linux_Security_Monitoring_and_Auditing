## Overview
This repository contains my Week 4 laboratory for Linux Security Monitoring and Auditing, completed as part of the International Cybersecurity and Digital Forensics Academy (ICDFA) GRC102 programme. The laboratory demonstrates how Linux evidence can be collected, analyzed, and translated into security governance and control assurance.

## Objectives
1. Monitor Linux security events using auditd and journalctl.
   
2. Review audit rules, sensitive file activity, program execution, and authentication events.
   
3. Conduct a system security assessment using Lynis.
   
4. Identify security control weaknesses and document their governance significance.
   
5. Map findings to owners, risks, remediation actions, closure evidence, and retesting requirements.
   
6. Demonstrate how Linux evidence can support SIEM, continuous monitoring, and GRC assurance.

## Findings
The auditd review confirmed that the service was active and custom audit rules were loaded. Audit records provided evidence of activity involving /etc/passwd, program execution, and authentication events.

Linux log analysis identified system activity, warnings, errors, privilege-use events, and a sudo authentication failure followed by successful privileged activity. The event was treated as a monitoring concern requiring context and correlation rather than proof of malicious activity.

The Lynis assessment identified hardening opportunities, including firewall configuration, Fail2ban, GRUB protection, password controls, centralized logging, and file permissions. The FIRE-4512 firewall finding required validation against the actual firewall architecture before remediation.

Governance & Assurance

The laboratory shows the flow from technical evidence → monitoring → investigation → GRC finding → remediation → retesting → closure. It highlights how security monitoring can provide evidence for control effectiveness, risk management, governance escalation, and continuous security assurance.
