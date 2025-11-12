# Layer 4: Transport Layer

## Role and Responsibilities
- Ensures end-to-end communication between applications on different devices.
- Provides reliability, error recovery, and flow control.
- Segments data into smaller units called segments.

## Key Functions
- Segmentation & Reassembly: Breaks large data into smaller segments and reassembles at destination.
- Error Detection & Recovery: Ensures data integrity.
- Flow Control: Prevents sender from overwhelming receiver.
- Connection Management: Establishes and terminates sessions (TCP handshake).

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
