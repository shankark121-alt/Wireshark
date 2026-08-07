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
Part 1:Start Kali Linux in Vmware and open the terminal and type sudo wireshark. Wireshark window is open in the command prompt type sudo wireshark.

Description:

This screenshot demonstrates launching Wireshark from the Kali Linux terminal using root privileges (sudo wireshark) to ensure the application 
has administrative access to interface adapters.It shows the selection of the active network interface (eth0) to begin live packet capturing across 
the local network.It serves as the initial setup phase where raw network packets are intercepted before applying specific display filters.

<img width="1280" height="658" alt="image" src="https://github.com/user-attachments/assets/35259f34-b008-4d31-a3ff-e67b925c0450" />

Part 2: 
2. Description for Screenshot 2 (Traffic Analysis & Color-Coded Windows Server IP Traffic)
Title: Real-Time Traffic Analysis and Color-Coded Packets for Windows Server IP (192.168.190.134)

Description:

This screenshot captures live network traffic passing through the interface, highlighting communication involving the Windows Server 2022.

** Green / Teal Rows:** Represent active and successful TCP data transmission, HTTP traffic, and Acknowledgments (ACK) packets flowing between the host
  and external servers.
** Yellow Rows:** Indicate connection setup flags (such as `[SYN]`, `[SYN, ACK]`) or specific handshake markers during the initial TCP connection phase.
** Grey Rows:** Highlight secure TLS/SSL encrypted sessions (such as `Client Hello`, `Server Hello`, and certificate exchanges) or connection teardown packets 
   (`[FIN, ACK]`).
** Red Rows:** Indicate TCP Reset (`[RST, ACK]`) packets showing where connections were abruptly terminated, aborted, or reset by the system or application.

<img width="1278" height="672" alt="image" src="https://github.com/user-attachments/assets/8e1d879f-9ee7-4030-9d78-e3c82c676a97" />
<img width="1277" height="654" alt="image" src="https://github.com/user-attachments/assets/b2ee196a-f5f3-4232-b7e6-9c70c14d86bc" />
<img width="1280" height="663" alt="image" src="https://github.com/user-attachments/assets/cce48cb9-ddd8-45b5-9612-68cf28d9cc7b" />






