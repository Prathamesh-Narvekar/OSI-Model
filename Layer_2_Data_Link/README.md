# Layer 2: Data Link Layer

## Role and Responsibilities
- Provides node-to-node delivery over the same physical network using MAC address.
- Ensures error detection and correction for frames.
- Handles MAC addressing for identifying devices on the same network segment.
- Organizes data into frames for transmission.

## Key Functions
### Framing
Converts raw bits from the Physical Layer into structured frames (packets with headers and trailers) and converts packets from Layer 3 into frames for transmission.

### Error Detection
  - Error detection techniques allow the receiver to identify if the received frame has errors before processing it. When data travels across a network, it can get corrupted due to:
    - Noise in the transmission medium
    - Signal attenuation
    - Interference
  - How It Works
    - The sender adds redundant bits (called error-detecting codes) to the data frame.
    - The receiver uses these bits to check if the data is intact.
    - If an error is detected, the frame is discarded or a retransmission is requested (depending on the protocol).
  - Common Error Detection Methods
    - Parity Check
    - Cheksum
    - Cyclic Redundancy Check (CRC)  
### Flow Control
  - Prevents overwhelming the receiver.
  - The sender sends data only as fast as the receiver can handle.
  - It prevents congestion and maintains reliable communication.
  - Techniques Used
    - Stop-and-Wait Protocol
    - Sliding Window Protocol
    - Go-Back-N Protocol
    - Selective Repeat  

### MAC Addressing 
A MAC Address (Media Access Control Address) is a unique hardware identifier assigned to a network interface card (NIC) for communication at the Data Link Layer of the OSI model.

### Access Control
  - Access Control in the Data Link Layer refers to the mechanism that determines which device gets to use the shared communication medium when multiple devices are connected to the same network segment (like in LANs). This is crucial because if two devices transmit at the same time, it causes collisions and data loss.
  - Why Access Control is Needed
    - In networks like Ethernet or Wi-Fi, many devices share the same physical medium.
    - Without coordination, simultaneous transmissions lead to collision and retransmission, reducing efficiency.
  - Access Control Methods
    - CSMA/CD (Carrier Sense Multiple Access with Collision Detection) – Used in wired Ethernet.
      - Device listens to the channel before sending.
      - If collision occurs, devices stop and retry after a random delay.
    - CSMA/CA (Carrier Sense Multiple Access with Collision Avoidance) – Used in Wi-Fi.
      - Tries to avoid collisions by waiting for a clear channel and using acknowledgments. 
 

## Devices at Data Link Layer
- Switches
  - Role: Forward frames based on MAC addresses.
  - Why Important: Reduces collisions compared to hubs; creates separate collision domains.
  - Example: Cisco Catalyst Switch in LAN.
- Bridges
  - Role: Connect two LAN segments and filter traffic using MAC addresses.
  - Why Important: Used in older networks; modern switches perform bridging internally.
- NIC (Network Interface Card)
  - Role: Hardware inside your computer that implements Layer 2 functions (MAC address, framing).
  - Why Important: Every device needs a NIC to connect to a network.
- Wireless Access Points (APs)
  - Role: Provide wireless connectivity; operate at Layer 2 for frame handling.
  - Why Important: Essential for Wi-Fi networks.

## Standards
- IEEE 802.3: Ethernet standard.
- IEEE 802.11: Wireless LAN (Wi-Fi).
- IEEE 802.1Q: VLAN tagging.
- PPP (Point-to-Point Protocol): Used in WAN links.

## Common Issues
- MAC Address Conflicts: Two devices with the same MAC.
- Switching Loops: Caused by redundant links (fixed by STP).
- Frame Errors: CRC failures due to interference or faulty NIC.
- Broadcast Storms: Excessive broadcast traffic flooding the network.
- VLAN Misconfiguration: Incorrect VLAN assignments causing connectivity issues.

## Real-World Examples
- Ethernet LAN communication.
- Wi-Fi data transfer between devices.
- VLAN segmentation in enterprise networks.
