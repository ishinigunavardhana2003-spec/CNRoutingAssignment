Router Configuration & Routing Protocols SimulationThis repository contains Cisco Packet Tracer simulation files demonstrating basic device security, manual static routing, and dynamic routing implementations (RIPv2 and EIGRP) across a three-subnet topology. File DescriptionsThis repository contains three independent network simulation files:Static_Routing_Configuration.pkt – Network connectivity established using manually configured static routes (ip route).  RIPv2_Dynamic_Routing.pkt – Dynamic routing implemented via Routing Information Protocol (RIPv2) with classless routing enabled.  EIGRP_Dynamic_Routing.pkt – Optimized dynamic routing using Enhanced Interior Gateway Routing Protocol (EIGRP AS-100) for fast convergence.   Quick-Reference Commands1. Device Security & Identity (Task 1)PlaintextRouter(config)# hostname HomagamaNSBM_39310
Router(config)# line console 0
Router(config-line)# password NSBM
Router(config-line)# login
Used to identify the device and protect physical console access.  2. Dynamic Routing Protocols (Task 3)RIPv2:PlaintextRouter(config)# router rip
Router(config-router)# version 2
Router(config-router)# network173.16.0.10

Router(config-router)# no auto-summary
*   **EIGRP (AS 100):**
    ```text
    Router(config)# router eigrp 100
    Router(config-router)# network [network-address]
    Router(config-router)# no auto-summary
 How to Run & VerifyDownload and install Cisco Packet Tracer.Clone this repository or download the .pkt files.Open any of the three lab files inside Packet Tracer.Open a device CLI and use the ping command to verify end-to-end connectivity.  Use the show ip route command on any router to inspect its live routing table.  Student DetailsStudent Name: P V T I K Gunavardhana Student ID: 39310  Module: Computer Networks  Assignment Template Reference: CN_Routing_Assignment_Report_Template.docx
