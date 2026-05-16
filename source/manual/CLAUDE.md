# docs/source/manual — End-User Manual

Up: [`../CLAUDE.md`](../CLAUDE.md) · [`../../../CLAUDE.md`](../../../CLAUDE.md)

---

Per-feature `.rst` pages covering OPNsense from an operator's perspective.
Read these **first** when reasoning about how a feature is supposed to be
configured.

## High-Value Pages

| File | Topic |
|---|---|
| `dashboard.rst` | Dashboard widgets and customization. |
| `gui.rst` | GUI conventions, ACL, theme. |
| `firewall.rst`, `firewall_generic.rst`, `firewall_categories.rst`, `firewall_groups.rst`, `firewall_settings.rst`, `firewall_scrub.rst`, `firewall_vip.rst`, `diagnostics_firewall.rst` | `pf` rules, NAT, scrub, VIPs. |
| `aliases.rst` | Firewall aliases (used in rules). |
| `interfaces.rst`, `interfaces_assignments.rst`, `interfaces_*.rst`, `diagnostics_interfaces.rst` | Interface modeling and live diagnostics. |
| `dhcp.rst`, `dnsmasq.rst`, `dhcrelay.rst`, `kea.rst` | DHCP services (legacy + modern). |
| `unbound.rst`, `unbound-dnsbl.rst` | DNS resolver. |
| `dynamic_dns.rst`, `dynamic_routing.rst` | Dynamic DNS and routing. |
| `gateways.rst` | Gateway management. |
| `vpn-*.rst`, `ipsec*.rst`, `openvpn*.rst`, `wireguard.rst` | VPN protocols. |
| `captiveportal.rst` | Captive portal. |
| `certificates.rst`, `git-backup.rst`, `backups.rst` | Trust store and backup. |
| `antivirus.rst`, `etpro_telemetry.rst`, `ids.rst`, `suricata*.rst` | Threat protection. |
| `hardware.rst`, `cpu-microcode.rst` | Hardware notes. |
| `users-and-groups.rst`, `auth*.rst` | Identity. |
| `monitoring.rst`, `monit.rst`, `netflow*.rst`, `rrd.rst` | Monitoring. |
| `firmware.rst`, `releases.rst` | Firmware lifecycle. |
| `how-tos/` | Recipe-style how-to pages. |

## Working Rules

- Read-only vendor source.
- When OPNsense's exact behavior conflicts with these docs, file an upstream
  issue rather than silently treating either as authoritative — they
  drift on edges, and the upstream community resolves the gap.
