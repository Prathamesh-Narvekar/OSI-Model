# Layer 2: Data Link Layer

## Role and Responsibilities
- Provides node-to-node communication over the same physical network.
- Ensures error detection and correction for frames.
- Handles MAC addressing for identifying devices on the same network segment.
- Organizes data into frames for transmission.

## Key Functions
- Framing: Converts packets from Layer 3 into frames for transmission.
- Error Detection: Uses techniques like CRC (Cyclic Redundancy Check).
- Flow Control: Prevents overwhelming the receiver.
- MAC Addressing: Unique hardware address for each device.
- Access Control: Determines which device can use the network medium (CSMA/CD, CSMA/CA).

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
