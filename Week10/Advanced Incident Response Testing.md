# [Advanced Incident Response Testing]([Security Incident Response Testing To Meet Audit Requirements | Infosec Resources (infosecinstitute.com)](https://resources.infosecinstitute.com/topic/incident-response-and-audit-requirements/))

## Introduction

- Incident response teams in enterprise environments must conduct drills to meet regulatory requirements and keep incident handlers sharp.
- PCI-DSS 12.9 outlines specific incident response plan requirements and testing procedures.

## Minimum Requirements for Testing Success

- Documented incident response plan aligned with NIST SP800-61 and updated regularly.
- 24/7 availability of incident response personnel.
- Monitoring mechanisms in place (IDS, IPS, FIMs) with regular alerts.
- Moderate level of technical incident response capability.

## Recommendations for Incident Response Drills

- Conduct quarterly testing instead of just annual testing to improve incident response capabilities.
- Fully document and report the drill process with methods, timelines, participants, and findings.
- Establish mandatory roles (moderator, coordinator, testers) and an optional observer for the drill.

## Incident Response Testing Steps

- Select target system(s) in advance, preferably one or two hosts that are in scope for PCI-DSS compliance.
- Prepare the target system by compromising it in a controlled manner, introducing a Trojan backdoor.
- Use various tactics and tools (e.g., netcat, cryptcat, Tini) to compromise the system and trigger alerts from monitoring systems.
- Hide the backdoor in a non-obvious location, challenging incident handlers to find it through analysis.
- Optionally, turn the backdoor into a service named after a known good system process to further challenge handlers.
- Connect to the backdoor just before the test period starts, leaving a network stack bread crumb trail.
- Escalate the "compromise" according to the incident response plan, allowing handlers a limited time window to identify the root cause.
- Ensure handlers remove the backdoor and clean up the system, documenting the process and lessons learned.

## Reporting Guidelines

- Create a clean, legible, and audit-worthy report documenting the entire incident response testing process.
- Include details of the test, roles, findings, cleanup process, and lessons learned.
- Emphasize the post-mortem meeting and improvements made based on lessons learned.

Incident response testing is crucial for validating incident response capabilities, meeting compliance requirements, and continuously improving the incident response process. By conducting regular drills and documenting the outcomes, organizations can strengthen their incident response capabilities and effectively respond to security incidents.