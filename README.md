# Introduction to Wireshark

Wireshark is the world's most widely used network protocol analyzer. It captures live traffic running on a network interface and allows you 
to inspect every single packet at a microscopic level. In cybersecurity and network administration, it is used for troubleshooting, traffic analysis, 
and detecting malicious or suspicious activity

# Step-by-Step Description of Wireshark Practical Topics
1. Packet Capture
Description: This is the first and primary step in Wireshark where raw packets flowing through the network interface card (such as eth0 seen in the capture)
are intercepted.
2. TCP Handshake
Description: A 3-Way Handshake is used to establish a TCP connection, during which SYN, SYN-ACK, and ACK packets are exchanged.
3. DNS (Domain Name System)
Description: DNS translates human-readable domain names into machine-readable IP addresses.
Generate traffic using the nslookup or dig command in the terminal, and analyze the query and response in Wireshark by applying the dns filter.
4. HTTP / HTTPS
Description: These are the primary protocols used for web traffic. HTTP transmits data in plain text, whereas HTTPS is secure and encrypted using TLS/SSL.
The capture clearly displays HTTP requests for Microsoft update files over port 80.
5. ICMP (Internet Control Message Protocol)
Description: ICMP is utilized for network diagnostics and error reporting. Running a ping command generates ICMP Echo Request and Echo Reply packets.
6. FTP (File Transfer Protocol)
Description: FTP is used for transferring files between servers across a network. Standard FTP transmits user credentials (usernames and passwords) in clear
text.
7. Attack Analysis
Description: This step involves identifying cyber attacks or network anomalies, such as Port Scans (Nmap) or abrupt connection drops. For instance, packet no.
20 displays a [RST, ACK] (Reset flag), indicating that the connection was forcefully terminated or reset.

# Practical Steps to perform wireshark practical
Part 1: Description of Your Two Screenshots (For your Practical Report / README.md)
Aap apni GitHub repository ki README.md file ya practical report me in descriptions ko add kar sakte hain:

1. Description for Screenshot 1 (sudo wireshark / Live Packet Capture Initialization)
Title: Launching Wireshark with Root Privileges

Description:

This screenshot demonstrates launching Wireshark from the Kali Linux terminal using root privileges (sudo wireshark) to ensure the application 
has administrative access to interface adapters.It shows the selection of the active network interface (eth0) to begin live packet capturing across 
the local network.It serves as the initial setup phase where raw network packets are intercepted before applying specific display filters.

