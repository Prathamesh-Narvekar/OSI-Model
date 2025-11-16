# Layer 4: Transport Layer
The Transport Layer (Layer 4) is the crucial layer that manages the entire data transfer process between two specific applications—not just two computers—across a network. It's the network's quality assurance and delivery service.

### Guaranteeing Application-to-Application Delivery
- Think of the Transport Layer as the postal service for your applications. When you send a large package (data) from one office to another, Layer 4 handles the logistics:
  - Addressing the Recipient (Port Numbers): It doesn't just address the city (computer's IP address, Layer 3); it addresses the specific person/department inside the building (the port number, which identifies the application like a web browser or email program). This is called multiplexing.
  - Choosing the Service: It lets you choose between a reliable, tracked service (TCP) or a fast, best-effort service (UDP).
  - Ensuring Integrity: It guarantees that all parts of the package arrive and are put back together correctly.
## Role and Responsibilities
- Ensures end-to-end communication between applications on different devices.
- Provides reliability, error recovery, and flow control.
- Segments data into smaller units called segments.

## Key Functions

### Segmentation & Reassembly
- This is necessary because network hardware has size limitations (like an envelope size).
- How it Works: The Transport Layer takes a large block of data from Layer 5 and breaks it into smaller, manageable pieces called segments. Each segment is numbered. At the destination, the layer uses these numbers to put the segments back in the correct order, even if they arrived out of sequence.

### Choosing Delivery Type (Protocols)
- This determines the level of reliability for the transfer.
  - TCP (Transmission Control Protocol): Used when reliability is paramount (e.g., file transfers, web browsing). TCP is connection-oriented: it establishes a formal connection (handshake), acknowledges every segment received, and resends any that are lost.
  - UDP (User Datagram Protocol): Used when speed is more important than guaranteed delivery (e.g., live video streaming, online gaming). UDP is connectionless: it just sends the data and doesn't check if it arrives.

### Flow Control
- This prevents the faster sender from overwhelming the slower receiver.
-  How it Works: The receiver constantly tells the sender how much data buffer space it has left (windowing). If the receiver gets busy, it can tell the sender to slow down or temporarily stop transmitting, preventing data from being dropped and lost.

### Error Detection & Recovery
- This ensures the data is received exactly as it was sent.
- How it Works (TCP): The receiver checks each segment for corruption (using a checksum). If an error is detected or if a segment doesn't arrive in time, the receiver simply doesn't acknowledge it. The sender then automatically retransmits the missing or damaged segment.

## Devices at Transport Layer
_(Transport Layer is mostly software-based, not hardware-specific, but these apply indirectly)_
- Gateways: Translate between different transport protocols.
- Firewalls (Transport Layer): Filter traffic based on port numbers.

## Standards & Protocols
- TCP (Transmission Control Protocol): Reliable, connection-oriented.
- UDP (User Datagram Protocol): Fast, connectionless, no reliability.
- SCTP (Stream Control Transmission Protocol): Used in telecom signaling.
- Ports:
  - Well-known ports (HTTP: 80, HTTPS: 443, FTP: 21).

## Common Issues
- Port Blocking: Firewalls blocking required ports.
- Connection Drops: TCP session termination issues.
- High Latency: Affects TCP performance.
- Packet Loss: Causes retransmissions and slowdowns.

## Real-World Examples
- TCP: Web browsing, email (HTTP, SMTP).
- UDP: Video streaming, VoIP, gaming.
- SCTP: Telecom signaling.
