# Task 4: Setup and Use a Firewall on Windows

## Objective
Configure and test basic Windows Firewall rules to allow or block specific ports, demonstrating how traffic can be filtered for enhanced security.

## Tools Used
- **Operating System**: Windows 11
- **Firewall Tool**: Windows Defender Firewall with Advanced Security
- **Command Prompt**: For testing connectivity using `telnet`

## Steps Followed
1. Opened Windows Defender Firewall with Advanced Security.
2. Viewed existing inbound firewall rules.
3. Created a new rule to block TCP traffic on port 23 (Telnet).
4. Verified the block by testing with `telnet localhost 23`.
5. Added a rule to allow TCP traffic on port 22 (SSH).
6. Tested SSH rule (optional, if OpenSSH server was active).
7. Removed the test rule to restore original configuration.

## Firewall Rule Summary

| Rule Name             | Action  | Port | Protocol | Profile              |
|-----------------------|---------|------|----------|----------------------|
| Block Telnet Port 23  | Block   | 23   | TCP      | Domain, Private, Public |
| Allow SSH Port 22     | Allow   | 22   | TCP      | Domain, Private, Public |

## Screenshots Included
- Creating the Telnet block rule
- Testing `telnet localhost 23`
- Creating the SSH allow rule
- Rule list showing both firewall rules

## Conclusion
This task showed how to use Windows Firewall to block unsafe ports, allow secure ones, test settings, and understand how it protects the system by controlling network traffic.
