# Data Flow in OSI Model

## What is Data Flow?
Data flow refers to how information moves from the Application Layer of the sender down to the Physical Layer, across the network, and then back up to the Application Layer of the receiver.

## Encapsulation Process (Sender Side)
When data is sent:
- Application Layer (Layer 7): Creates the message (e.g., HTTP request).
- Presentation Layer (Layer 6): Formats, encrypts, compresses data.
- Session Layer (Layer 5): Establishes session and adds session info.
- Transport Layer (Layer 4): Breaks data into segments, adds TCP/UDP header.
- Network Layer (Layer 3): Adds IP header, creating a packet.
- Data Link Layer (Layer 2): Adds MAC header and trailer, creating a frame.
- Physical Layer (Layer 1): Converts frame into bits and transmits as signals.
Result: Data is fully encapsulated with headers (and sometimes trailers) from each layer.

## Decapsulation Process (Receiver Side)
When data is received:
- Physical Layer: Converts signals back into bits.
- Data Link Layer: Removes MAC header/trailer, passes packet up.
- Network Layer: Removes IP header, passes segment up.
- Transport Layer: Reassembles segments, removes TCP/UDP header.
- Session Layer: Synchronizes and manages session.
- Presentation Layer: Decrypts, decompresses, translates data.
- Application Layer: Delivers the original message to the application.
Result: Original data is reconstructed for the user.

## PDU Transformation
| Layer | PDU Name |
| --- | --- |
| Application | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

## Real-World Example
Sending an email:
- You type an email → Application Layer.
- It’s formatted and encrypted → Presentation Layer.
- Session established → Session Layer.
- TCP segments created → Transport Layer.
- IP packets formed → Network Layer.
- Ethernet frames created → Data Link Layer.
- Bits transmitted over cable → Physical Layer.
