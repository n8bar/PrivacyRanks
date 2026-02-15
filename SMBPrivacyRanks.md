# SMB / IT / MSP Privacy & Security Ranks (16 Ranks)

## 1) Asset Steward
**Core Move:** Maintain an accurate inventory of devices, accounts, and SaaS.  
**Unlock Requirement:** A single source of truth for hardware, users, and core services.  
**Daily Habit:** Update inventory whenever a device or account is added/removed.  
**Payoff:** ROI: High | Effort: Low  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is "you can't secure what you can't see." Without this, every other control is partially blind and risk stays high.  
**Boss Fight:** Shadow IT and unknown admin accounts.

## 2) Patch Captain
**Core Move:** Patch OS, browsers, and critical apps on a fixed cadence.  
**Unlock Requirement:** A patch schedule and owner with visibility into compliance.  
**Daily Habit:** Apply critical updates quickly; verify completion.  
**Payoff:** ROI: High | Effort: Medium  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is "known vulnerabilities are optional" - and they choose not to be exposed. Without it, commodity exploits stay effective.  
**Boss Fight:** Deferred updates that become permanent backlog.

## 3) Identity Gatekeeper
**Core Move:** Enforce MFA on all critical services and admin accounts.  
**Unlock Requirement:** MFA coverage for email, admin consoles, and financial systems.  
**Daily Habit:** Require MFA for new accounts and vendors by default.  
**Payoff:** ROI: High | Effort: Medium  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is "passwords are not a control by themselves." Without MFA, account takeover remains a top breach path.  
**Boss Fight:** SMS-only MFA or inconsistent enforcement.

## 4) Password Vault
**Core Move:** Use a team password manager with unique credentials.  
**Unlock Requirement:** Shared vaults with access controls and audit trails.  
**Daily Habit:** Generate passwords and revoke access promptly.  
**Payoff:** ROI: High | Effort: Medium  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is credential discipline at scale. Without it, one leak or reuse incident can cascade across systems.  
**Boss Fight:** Shared passwords in docs or chat.

## 5) Email Shield
**Core Move:** Harden email with SPF/DKIM/DMARC and phishing defenses.  
**Unlock Requirement:** DMARC policy set and phishing reporting flow in place.  
**Daily Habit:** Monitor failed auth reports and adjust rules.  
**Payoff:** ROI: High | Effort: Medium  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is "email is the front door." Without this, spoofing and business email compromise remain easy.  
**Boss Fight:** No DMARC enforcement or ignored alerts.

## 6) Backup Warden
**Core Move:** Implement 3-2-1 backups with tested restores.  
**Unlock Requirement:** At least one offline or immutable backup and monthly restore tests.  
**Daily Habit:** Verify backup success and storage capacity.  
**Payoff:** ROI: High | Effort: Medium  
**Who should do this:** Everyone  
**Rank Description:** Their attitude is resilience over hope. Without it, ransomware or accidental deletion can be fatal.  
**Boss Fight:** Backups that have never been tested.

## 7) Endpoint Sentinel
**Core Move:** Deploy modern endpoint protection (EDR/AV) with policy control.  
**Unlock Requirement:** Coverage on all endpoints with centralized alerts.  
**Daily Habit:** Review high-severity alerts and isolate suspicious devices.  
**Payoff:** ROI: Medium | Effort: Medium  
**Who should do this:** Most People  
**Rank Description:** Their attitude is "assume compromise." Without it, detection and containment are delayed.  
**Boss Fight:** Alerts ignored due to noise.

## 8) Least-Privilege Marshal
**Core Move:** Enforce least privilege and role-based access.  
**Unlock Requirement:** Defined roles and removal of unnecessary admin rights.  
**Daily Habit:** Approve access only when justified and time-bound.  
**Payoff:** ROI: Medium | Effort: Medium  
**Who should do this:** Most People  
**Rank Description:** Their attitude is reducing blast radius. Without it, one compromised account can access everything.  
**Boss Fight:** All-staff admin access.

## 9) Network Cartographer
**Core Move:** Segment networks (guest, staff, servers, IoT) and lock down routers.  
**Unlock Requirement:** Separate VLANs/SSIDs and hardened network gear.  
**Daily Habit:** Review new devices and isolate unknowns.  
**Payoff:** ROI: Medium | Effort: Medium  
**Who should do this:** Most People  
**Rank Description:** Their attitude is containment by design. Without it, lateral movement is easy.  
**Boss Fight:** Flat networks with shared credentials.

## 10) Secure Access Operator
**Core Move:** Use secure remote access (VPN or zero-trust) and disable legacy protocols.  
**Unlock Requirement:** MFA-protected remote access with logging.  
**Daily Habit:** Review access logs and revoke stale accounts.  
**Payoff:** ROI: Medium | Effort: Medium  
**Who should do this:** Most People  
**Rank Description:** Their attitude is "remote access is privileged access." Without it, exposed services become easy targets.  
**Boss Fight:** RDP or admin portals exposed to the public internet.

## 11) Logkeeper
**Core Move:** Centralize logs and define alert thresholds.  
**Unlock Requirement:** Log aggregation for endpoints, email, and admin consoles.  
**Daily Habit:** Triage high-severity alerts and verify anomalies.  
**Payoff:** ROI: Medium | Effort: High  
**Who should do this:** Targeted  
**Rank Description:** Their attitude is "if you can't see it, you can't fix it." Without it, incidents are discovered too late.  
**Boss Fight:** Logs collected but never reviewed.

## 12) Incident Commander
**Core Move:** Maintain an incident response plan with owner roles.  
**Unlock Requirement:** A tested playbook for phishing, ransomware, and account takeover.  
**Daily Habit:** Keep contacts and escalation paths current.  
**Payoff:** ROI: Medium | Effort: High  
**Who should do this:** Targeted  
**Rank Description:** Their attitude is practiced response, not improvisation. Without it, downtime and losses grow.  
**Boss Fight:** No clear decision authority in a crisis.

## 13) Vendor Guardian
**Core Move:** Vet vendors/MSPs and define security expectations.  
**Unlock Requirement:** Security clauses, access limits, and offboarding steps.  
**Daily Habit:** Review vendor access and shared data quarterly.  
**Payoff:** ROI: Medium | Effort: High  
**Who should do this:** Targeted  
**Rank Description:** Their attitude is supply-chain awareness. Without it, third parties become the weakest link.  
**Boss Fight:** Permanent vendor access with no audits.

## 14) Data Steward
**Core Move:** Classify data and set retention/deletion rules.  
**Unlock Requirement:** Clear categories (public, internal, confidential) with handling rules.  
**Daily Habit:** Delete what you no longer need; reduce data exposure.  
**Payoff:** ROI: Medium | Effort: High  
**Who should do this:** Targeted  
**Rank Description:** Their attitude is "less data, less risk." Without it, breaches expose more than necessary.  
**Boss Fight:** Keeping sensitive data forever.

## 15) Training Guild
**Core Move:** Run ongoing security awareness and phishing simulations.  
**Unlock Requirement:** Quarterly training and measured improvement.  
**Daily Habit:** Reinforce one actionable habit per month.  
**Payoff:** ROI: Medium | Effort: High  
**Who should do this:** Targeted  
**Rank Description:** Their attitude is culture as a control. Without it, human error remains the dominant breach path.  
**Boss Fight:** One-time training with no reinforcement.

## 16) Resilience Architect
**Core Move:** Maintain business continuity and disaster recovery plans.  
**Unlock Requirement:** Tabletop exercises and recovery time objectives defined.  
**Daily Habit:** Review critical dependencies and recovery readiness.  
**Payoff:** ROI: High | Effort: High  
**Who should do this:** High-Risk  
**Rank Description:** Their attitude is survival under adverse conditions. Without it, a major incident can end the business.  
**Boss Fight:** Plans that exist only on paper.
