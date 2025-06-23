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
