# Phase 1 — Foundations

**Suggested pace:** 8–12 weeks, 6–10 hours/week. The checkpoint is explaining
how a request travels from a process to a service and how to investigate it.

## Domains

Detailed companion guides: [networking](../../domains/networking/README.md)
and [Linux/Windows](../../domains/linux-windows/README.md).

### Computing and operating systems
Processes/threads, memory and storage, boot, virtualization, users/groups,
permissions, package management, and system logs. Install a Linux VM and learn
the Windows security and event-log model.

### Networking
Binary and IPv4/IPv6 addressing, subnetting, routing, ARP/NDP, TCP/UDP, DNS,
HTTP(S), SSH, email, firewalls, NAT and TLS at a conceptual level. Capture only
your own traffic with Wireshark and explain a TCP handshake.

### Linux and Windows administration
Use shells, services, scheduled tasks, environment variables, SSH/WinRM,
PowerShell, least privilege, backups, and patching. Practice reading
`auth.log`/journald and Windows Event Viewer without changing production data.

## Labs and evidence

- Build two VMs on a host-only network; snapshot before experiments.
- Harden SSH/RDP, create a least-privilege account, and record the change.
- Capture a DNS lookup and HTTPS connection; annotate the packets.
- Write five small Bash or PowerShell scripts with input validation and logs.

**Checkpoint:** a one-page network diagram, a troubleshooting runbook, and a
short log-analysis report. Use [the progress template](../../templates/progress.md).

## Reliable references

[Linux Documentation](https://www.kernel.org/doc/html/latest/),
[Microsoft Learn security](https://learn.microsoft.com/security/),
[Cisco networking basics](https://www.cisco.com/c/en/us/solutions/enterprise-networks/what-is-computer-networking.html),
[Wireshark User's Guide](https://www.wireshark.org/docs/wsug_html/).
