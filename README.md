# -Task-1-Network-Port-Scanning
network-port-scan

## Tools Used
- Nmap
- Wireshark (optional)

Nmap installation

<img width="1404" alt="Screenshot 2025-06-23 at 9 04 16 PM" src="https://github.com/user-attachments/assets/8e0f76f4-c47a-4889-bf00-9dea504a176d" />
## Commands Used for Scanning
nmap -sS 192.168.1.0/24 -oN local_scan_results.txt

In nmap -sS scn stands for The -sS option in Nmap stands for TCP SYN scan.
i dont got any open ports and the command didnt worked at well i attached the text file
This is also known as a "half-open" scan because Nmap sends a SYN packet (used to initiate a TCP connection), and based on the response, it determines the port status:

SYN-ACK received → Port is open.
RST received → Port is closed.
No response or ICMP unreachable → Port is filtered.

so the result of the previous command is not appropiate so i used thsi instead of that i used this command from my own and the target is my own system i attached the scan result as an .txt file
nmap -A  192.168.31.182  --min-rate=5000 -oN scan_results.txt

| Flag                   | Meaning                                                                  |
| ---------------------- | ------------------------------------------------------------------------ |
| `-A`                   | Enables OS detection, version detection, script scanning, and traceroute |
| `192.168.31.182`       | Target IP address                                                        |
| `--min-rate=5000`      | Sends packets as fast as possible (minimum 5000 packets per second)      |
| `-oN scan_results.txt` | Saves output in normal format to `scan_results.txt`                      |

i got some services and its version and os type and also the device information which is used to gather more info about the target system.
