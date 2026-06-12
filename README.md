 Project Overview
This project demonstrates a complete enterprise network topology designed and configured using Cisco Packet Tracer. It includes network segmentation, dynamic IP allocation, routing, internet connectivity, and robust security implementations.

Technologies & Protocols Implemented
VLANs & Inter-VLAN Routing:Segmented the network into multiple VLANs (10, 20, 30, 40, 50, 99) using a Layer 3 Core Switch (Cisco 3560).
Routing: Configured OSPF (Open Shortest Path First) for internal routing between the Core Switch and the Edge Router.
NAT (Network Address Translation): Implemented NAT Overload (PAT) on the Cisco 2911 router to allow internal VLANs to access the Internet (simulated via a Loopback interface).
Device Security: Secured routers and switches with encrypted privileged exec passwords, console passwords, VTY (Telnet/SSH) passwords, and MOTD banners.
Port Security:Configured access switches to prevent unauthorized access using MAC address sticky learning and violation shutdown modes.

How to Test the Network
1. Download the `.pkt` file from this repository.
2. Open it using Cisco Packet Tracer.
3. Open the Command Prompt on any end-user PC.
4. Test Inter-VLAN Routing: Ping another PC in a different VLAN (e.g., `ping 10.10.30.11`).
5. Test Internet Connectivity: Ping the simulated external network (e.g., `ping 8.8.8.8`).
6. Test Port Security:Connect a new device to an access switch port and observe the port automatically shutting down to prevent unauthorized access.
