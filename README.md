# Networking Basics #0

## Description
This project covers foundational computer networking concepts, including the OSI model, network architectures (LAN, WAN, Internet), MAC and IP addressing (IPv4 vs. IPv6), data transfer protocols (TCP and UDP), standard port numbers, and basic network troubleshooting tools like `ping`.

## Learning Objectives
At the end of this project, you should be able to explain without external reference:
- **OSI Model**: What it is, its 7 layers, and its organization from physical (Layer 1) to application (Layer 7).
- **Network Types**: Key characteristics, geographical scopes, and typical usage of LAN, WAN, and the Internet.
- **Addressing**: Physical MAC addresses, logical IP addresses, private vs. public IPs, `localhost` (`127.0.0.1`), subnets, and why IPv6 was introduced.
- **Transport Layer**: Fundamental differences between TCP (connection-oriented, reliable) and UDP (connectionless, fast).
- **Ports**: Function of network ports and standard port assignments (**SSH**: 22, **HTTP**: 80, **HTTPS**: 443).
- **Network Diagnostics**: Using ICMP and `ping` to verify host connectivity.

## General Requirements
- Allowed text editors: `vi`, `vim`, `emacs`
- All Bash script files are interpreted on **Ubuntu 22.04 LTS**
- All script files must be executable (`chmod +x <filename>`)
- All Bash scripts must pass `shellcheck` without any errors
- The first line of all Bash scripts must be exactly `#!/usr/bin/env bash`
- The second line of all Bash scripts must be a comment explaining what the script does
- Every file must end with a new line
- A `README.md` file at the root of the project directory is mandatory

## File Structure & Task Overview

| File | Description | Type |
| :--- | :--- | :--- |
| `0-OSI_model` | Questions on OSI model definitions and layer ordering | Answer File |
| `1-types_of_network` | Questions on LAN, WAN, and Internet characteristics | Answer File |
| `2-MAC_and_IP_address` | Questions on MAC addresses, IPv4/IPv6, subnets, and localhost | Answer File |
| `3-UDP_and_TCP` | Questions comparing TCP and UDP operational mechanics | Answer File |
| `4-TCP_and_UDP_ports` | Questions on network ports and standard service numbers | Answer File |
| `5-is_the_host_on_the_network` | Bash script that accepts an IP address as `$1` and pings it | Executable Bash Script |

---

### Task 5 Script Template (`5-is_the_host_on_the_network`)
```bash
#!/usr/bin/env bash
# Displays network connection status by pinging an IP address passed as a parameter
ping -c 5 "$1"
