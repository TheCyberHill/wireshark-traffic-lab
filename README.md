# wireshark-traffic-lab
Using Wireshark to capture and analyze traffic.

🕵️‍♂️ TCP Traffic Analysis Lab <br>
A hands-on exploration of suspicious TCP packets using Wireshark in a sandboxed VM.
Built to reinforce practical network defense techniques, anomaly detection, and log parsing workflows.

📦 Project Overview <br>
This lab simulates malicious or anomalous TCP traffic and walks through dissecting it using Wireshark. Traffic was generated using nc (Netcat) to create a controlled attack scenario—perfect for observing abnormal handshakes, unexpected payloads, and port activity in action.
📸 Screenshots included throughout the walkthrough provide visual context and help solidify key concepts.

🔧 Tools Used
- Wireshark: packet inspection and protocol dissection
- Kali Linux VM: controlled environment for safe experimentation
- Netcat (nc): traffic simulation and basic payload crafting
- Python (optional): for parsing and filtering logs

🎯 What I Learned
- TCP handshake patterns and anomalies
- Packet payload inspection and protocol behaviors
- Using Netcat to generate and manipulate TCP traffic
    - nc -l -p 4444
    - echo -e "GET /login.php HTTP/1.1\r\nHost: evil.local\r\nAuthorization: Basic YWRtaW46aHVudGVyMg==\r\n\r\n" | nc -nv <eth0_IP> 4444
- Identifying potentially malicious activity
- Using filters and display options effectively in Wireshark

🛠️ Lab Configuration
- Environment: Kali Linux VM
- Traffic Simulation: Netcat (nc) used to craft and send packets
- Capture Tool: Wireshark
- Screenshots: Embedded throughout to document key findings


💡 Why This Matters <br>
Network analysis is ground zero for threat detection. This lab emphasizes hands-on skills that mirror real-world investigative work—perfect for aspiring threat hunters or SOC analysts.

<img src="Wireshark1.png" width="500">
<img src="Wireshark2.png" width="500">
<img src="Wireshark3.png" width="500">
