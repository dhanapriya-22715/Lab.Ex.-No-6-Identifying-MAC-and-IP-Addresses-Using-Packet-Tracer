# Ex. No: 6 Identifying MAC and IP Addresses Using Packet Tracer
# Date:17/11/2026
________________________________________
# Objective
To use Cisco Packet Tracer simulation mode to capture and analyze MAC and IP address information for both local and remote network communication.
________________________________________
# Apparatus/Tools Required
•	Cisco Packet Tracer<br>
•	Pre-configured network topology (as provided in the activity file)<br>
•	PCs, switches, router, hub, and wireless access point (as per given setup)<br>
________________________________________
# Network Topology Diagram
# Description:
•	The topology contains a local network (172.16.31.0/24) connected to a remote network (10.10.10.0/24) via a router.<br>
•	Devices include PCs, switches, hub, and wireless AP.<br>
<img width="1917" height="1141" alt="image" src="https://github.com/user-attachments/assets/e273bfa4-6410-41e2-a5fc-0b8e23617cac" />

________________________________________
# IP Addressing Table
(Example – actual values from simulation)<br>
Device	IPv4 Address	Subnet Mask	MAC Address<br>
PC-A	172.16.31.5	255.255.255.0	00D0:D311:C788<br>
PC-B	172.16.31.2	255.255.255.0	000C:85CC:1DA7<br>
Router (G0/0)	172.16.31.1	255.255.255.0	00D0:BA8E:741A<br>
PC-Remote	10.10.10.2	255.255.255.0	00D0:588C:2401<br>
________________________________________
# Procedure
# Part 1: Local Network Communication
1.	Click PC-A (172.16.31.5) and open the Command Prompt.<br>
2.	Enter ping 172.16.31.2.<br>
3.	Switch to Simulation Mode and repeat the ping.<br>
4.	When the PDU appears, click it and record: Destination MAC, Source MAC, Source IP, Destination IP, and the device name.<br>
5.	Use Capture/Forward to follow the PDU through the network until it reaches PC-B.<br>
6.	Record the information in a table.<br>
7.	Repeat the above process for:<br>
o	Ping from 172.16.31.3 to 172.16.31.2<br>
o	Ping from 172.16.31.5 to 172.16.31.4<br>
Part 2: Remote Network Communication<br>
1.	From PC-A (172.16.31.5), enter ping 10.10.10.2.<br>
2.	Switch to Simulation Mode and repeat the ping.<br>
3.	When the PDU appears, note the Destination MAC, Source MAC, Source IP, and Destination IP.<br>
4.	Follow the PDU step-by-step until it reaches the remote PC.<br>
5.	Observe how MAC addresses change at the router while IP addresses remain constant end-to-end.<br>
________________________________________
# Example Data Recording Table
At Device	Dest. MAC	Src MAC	Src IPv4	Dest IPv4<br>
172.16.31.5	000C:85CC:1DA7	00D0:D311:C788	172.16.31.5	172.16.31.2<br>
Switch1	000C:85CC:1DA7	00D0:D311:C788	N/A	N/A<br>
172.16.31.2	00D0:D311:C788	000C:85CC:1DA7	172.16.31.2	172.16.31.5<br>
________________________________________
# Output (Screenshots)
•	PDU details for local communication<br>
<img width="1916" height="958" alt="image" src="https://github.com/user-attachments/assets/140d7848-eab8-45f4-a5c5-a870eea89ac0" />

<img width="1917" height="950" alt="image" src="https://github.com/user-attachments/assets/f7394084-9af5-4e6b-ab5d-27f92db2c933" />

<img width="1917" height="1000" alt="image" src="https://github.com/user-attachments/assets/bf4d6561-403e-4135-9d8b-31520366bf93" />


•	PDU details for remote communication<br>

<img width="1917" height="982" alt="image" src="https://github.com/user-attachments/assets/81d78826-728a-4687-8c58-43ad1b01879a" />


•	Tables showing MAC/IP changes through each device<br>

<img width="942" height="276" alt="image" src="https://github.com/user-attachments/assets/08ff6572-76cb-43d6-b979-e7ab36711841" />

________________________________________
# Result
Successfully captured and analyzed MAC and IP addresses for both local and remote communications. Verified that MAC addresses change at each hop while IP addresses remain constant from source to destination.
