# Layer 3: Network Layer

## Role and Responsibilities
- Handles logical addressing and routing of data between devices across multiple networks.
- Determines the best path for data to travel from source to destination.
- Organizes data into packets for transmission.

## Key Functions
- Routing: Chooses optimal path using routing algorithms.
- Logical Addressing: Assigns IP addresses to devices.
- Fragmentation & Reassembly: Splits large packets for transmission.
- Error Handling: Detects unreachable destinations (ICMP messages).

## Devices at Network Layer (Simplified & Practical)
- Routers
  - Role: Forward packets based on IP addresses.
  - Why Important: Connect different networks (LAN to WAN, LAN to Internet).
  - Example: Home broadband router or enterprise Cisco router.
- Layer 3 Switches
  -Role: Perform routing within LANs using IP addresses.
  Why Important: Combines switching and routing for high-speed internal networks.
- Firewalls (Network Layer)
  - Role: Filter traffic based on IP addresses and rules.
  - Why Important: Provides security by controlling which packets enter or leave the network.

## Standards
- IPv4 (Internet Protocol version 4)
  - Role: Provides logical addressing and routing for most networks.
  - Why Important: Still widely used despite IPv6 adoption.
  - Key Feature: 32-bit address space.
- IPv6 (Internet Protocol version 6)
  - Role: Successor to IPv4 with larger address space.
  - Why Important: Supports billions of devices and modern networking needs.
  - Key Feature: 128-bit address space.
- ICMP (Internet Control Message Protocol)
  - Role: Used for error reporting and diagnostics (e.g., ping).
  - Why Important: Helps troubleshoot connectivity issues.
- Routing Protocols
  - OSPF (Open Shortest Path First): Dynamic routing within large networks.
  - BGP (Border Gateway Protocol): Routing between ISPs and across the internet.
  - RIP (Routing Information Protocol): Simple distance-vector routing (legacy).

## Common Issues
- IP Address Conflicts: Two devices with same IP.
- Routing Loops: Incorrect routing table entries.
- Subnetting Errors: Misconfigured subnet masks.
- Packet Loss: Due to congestion or faulty routes.
- Incorrect Default Gateway: Device cannot reach outside network.

## Real-World Examples
- Internet communication between two websites.
- Routing in enterprise networks using OSPF or BGP.
- Ping command uses ICMP (Layer 3 protocol).

## Key Insight:
Network Layer = IP addressing + Routing. Without this layer, data cannot move beyond a local network.
