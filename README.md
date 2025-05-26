# nmap-wireshark

Installed Nmap on a Linux machine for network reconnaissance.

Identified local IP range (192.168.1.0/24) using the ip a command.

Performed a TCP SYN scan with:
sudo nmap -sS 192.168.1.0/24

Discovered an active Windows host (192.168.1.9) with ports 135, 139, and 445 open.

Detected services: Microsoft RPC, NetBIOS, and SMB.

Ran default Nmap vulnerability scripts on SMB ports; some scripts failed to negotiate due to firewall or SMB version issues.

Captured Nmap traffic using Wireshark on interface eth0.

Applied filters like ip.addr = 192.168.1.11 to  scan-related packets.

Saved the packet capture as a .pcapng file for further analysis and documentation.
