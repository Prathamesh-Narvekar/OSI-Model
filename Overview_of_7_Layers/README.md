# Overview of the 7 Layers
The OSI Model divides network communication into seven layers, each with a specific role. Here’s a structured view:

## Layer 1: Physical Layer
- Function: Deals with raw bit transmission over physical media.
- Key Responsibilities: Voltage levels, cables, connectors, data rates.
- Examples: Ethernet cables, fiber optics, hubs.
- PDU: Bits.

## Layer 2: Data Link Layer
- Function: Provides reliable node-to-node data transfer.
- Key Responsibilities: Framing, MAC addressing, error detection.
- Examples: Ethernet, PPP, Switches.
- PDU: Frame.

## Layer 3: Network Layer
- Function: Handles logical addressing and routing.
- Key Responsibilities: IP addressing, path selection.
- Examples: IP, ICMP, Routers.
- PDU: Packet.

## Layer 4: Transport Layer
- Function: Ensures end-to-end communication and reliability.
- Key Responsibilities: Segmentation, error recovery, flow control.
- Examples: TCP, UDP.
- PDU: Segment.

## Layer 5: Session Layer
- Function: Manages sessions between applications.
- Key Responsibilities: Session establishment, synchronization.
- Examples: NetBIOS, RPC.
- PDU: Data.

## Layer 6: Presentation Layer
- Function: Translates data formats, encryption, compression.
- Key Responsibilities: Data representation, security.
- Examples: SSL/TLS, JPEG, ASCII.
- PDU: Data.

## Layer 7: Application Layer
- Function: Provides network services to end-users.
- Key Responsibilities: Interface for applications.
- Examples: HTTP, FTP, SMTP, DNS.
- PDU: Data.

## Quick Summary Table

| Layer | Name | PDU | Protocols/Example |
| --- | --- | --- | --- |
| 7 | Application | Data | HTTP, FTP, DNS |
| 6 | Presentation | Data | SSL, JPEG |
| 5 | Session | Data | RPC, NetBIOS |
| 4 | Transport | Segment | TCP, UDP |
| 3 | Network | Packet | IP, ICMP, IGMP |
| 2 | Data Link | Frame | Ethernet, P2P |
| 1 | Physical | Bits | Cables, Hubs |
