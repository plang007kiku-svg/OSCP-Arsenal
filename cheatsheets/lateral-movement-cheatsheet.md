I. 🌐 Lateral Movement Attack

- Logic: Using the "root" (Root/Admin) machine as a base (Pivot) to penetrate the "internal subnet". [cite: 1.7]

- 1. Search for a new network. (Post-Exploitation Enum):

- View IP Address/Subnets: ip a or ifconfig (run on the server) [cite: 1000017371.jpg]
- View Gateway/Routing: route (run on the server) [cite: 1000017371.jpg]

- 2. Pivoting/Tunneling:

- Recommendation: A tunnel (e.g., Ligolo-ng, Chisel) must be created in Kali to send Nmap to the internal network (e.g., 192.168.10.0/24). [cite: 1.7]

- 3. Target Enumeration:

- Command: nmap -sV -T4 -Pn [Internal Subnet]/24 (e.g., 192.168.10.0/24) [cite: 1000017371.jpg]
- Purpose: Find Ports and Services running on the client machine [cite: 1.7]

II. 🛡️ Credential Attack (Lateral Attack)

- Logic: Use a HASH/Password stolen from the server [cite: 1000017441.heic] to try to log in directly to the client machine. [cite: 1000017441.heic]

- 1. Pass-the-Hash (SMB/Windows):

- Command: crackmapexec smb [client IP] -u [User] -H [HASH] [cite: 1000017441.heic]

- 2. SSH/RDP Logon:

- Command: ssh [User]@[client IP] or try logging in via RDP (Remote Desktop Protocol) [cite: 1000017441.heic]

- 3. Flag Proofing:

- Flag search: find / -name root.txt 2>/dev/null (run on the proofed client) [cite: 1.7]

Recommendation: Saving this information in Google Keep will allow you to access it instantly during the training! 
