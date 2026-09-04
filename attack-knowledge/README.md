# Attack knowledge, defensively framed

Understanding attacker behavior helps defenders prioritize controls. This
section describes **what to detect and prevent**, not instructions for harming
systems. Map observations to [MITRE ATT&CK](https://attack.mitre.org/) and
validate in a private lab.

| Behavior | Defensive questions |
| --- | --- |
| Initial access | Are exposed services inventoried, patched and protected by MFA? |
| Execution | Are scripts constrained and unusual parents logged? |
| Persistence | Are startup locations, identities and changes reviewed? |
| Credential access | Are secrets vaulted, short-lived and access-audited? |
| Discovery/lateral movement | Is east-west traffic limited and monitored? |
| Collection/exfiltration | Are sensitive stores classified and egress controlled? |
| Impact | Are immutable backups restored and recovery objectives tested? |

Use the [ATT&CK Enterprise matrix](https://attack.mitre.org/matrices/enterprise/)
and [CISA Known Exploited Vulnerabilities](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)
for prioritization. Do not publish real credentials, weaponized payloads, or
instructions targeting third-party systems.

## Learning levels

- **Beginner:** phishing, exposed services, weak passwords, unsafe
  configuration, and basic injection. Impact may include account or data
  exposure; indicators include authentication anomalies, repeated errors,
  unexpected configuration changes, and suspicious links. Detect with identity,
  endpoint, and application logs; prevent with MFA, patching, secure defaults,
  validation, and user reporting. Respond by scoping, containing, preserving
  evidence, resetting affected credentials, fixing the root cause, and
  verifying recovery.
- **Intermediate:** privilege escalation, persistence, lateral movement,
  cloud permission abuse, and supply-chain compromise. Impact can include
  broader access or service disruption; indicators include new services/tasks,
  unusual parent processes, policy changes, anomalous API calls, and unsigned
  artifacts. Detect with centralized telemetry and ATT&CK-mapped detections;
  prevent with least privilege, segmentation, signing, protected pipelines,
  and tested backups. Respond with approved isolation, token/key rotation,
  eradication, recovery, and lessons learned.
- **Advanced:** coordinated intrusion, destructive activity, data
  exfiltration, and abuse of OT or AI workflows. Impact may affect safety,
  availability, privacy, or trust; indicators include cross-source behavior
  chains, unusual egress, integrity failures, and control-plane anomalies.
  Detect through layered monitoring, threat intelligence, and independent
  recovery signals. Prevent with resilient architecture, deny-by-default
  controls, segmentation, offline recovery, and exercised crisis plans.
  Respond under the incident plan with clear authority, legal/privacy
  coordination, evidence integrity, safe containment, and validated restoration.

For every level, record IOC type, value or redacted representation, source,
time, affected asset, confidence, and TTP mapping. An IOC is a clue, not proof.
