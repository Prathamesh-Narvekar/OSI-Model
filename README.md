# OSI MODEL
The OSI (Open Systems Interconnection) Model is a conceptual framework that standardizes the functions of a communication system into seven distinct layers. Each layer has specific responsibilities, ensuring seamless data transmission between devices over a network. Below is an overview of the seven layers:  

**1. Physical Layer**  
This is the lowest layer, responsible for the actual physical connection between devices. It transmits raw bits (0s and 1s) over a communication medium like cables or wireless signals. It defines hardware specifications such as cables, connectors, and transmission modes (simplex, half-duplex, full-duplex).  

**2. Data Link Layer**  
This layer ensures node-to-node communication and error-free data transfer. It organizes data into frames and handles MAC (Media Access Control) and LLC (Logical Link Control). Devices like switches and bridges operate at this layer.  

**3. Network Layer**  
The network layer handles routing and addressing. It determines the best path for data to travel across networks using logical addresses (e.g., IP addresses). Routers operate at this layer, and data units are referred to as packets.  

**4. Transport Layer**  
This layer ensures end-to-end communication and reliable data delivery. It segments data into smaller units and reassembles them at the destination. Protocols like TCP (reliable) and UDP (unreliable) operate here.  

**5. Session Layer**  
The session layer manages sessions or connections between devices. It establishes, maintains, and terminates communication sessions. It also provides synchronization and checkpointing to ensure data integrity.  

**6. Presentation Layer**  
This layer acts as a translator, converting data into a format that the application layer can understand. It handles encryption, decryption, and compression. For example, it translates between ASCII and EBCDIC formats.  

**7. Application Layer**  
The topmost layer provides interfaces for end-user applications to access network services. Protocols like HTTP, FTP, SMTP, and DNS operate here, enabling tasks like file transfers, email, and web browsing.  

**Data Flow in the OSI Model**
When data is sent, it flows from the application layer (Layer 7) down to the physical layer (Layer 1) on the sender's side. At the receiver's end, the process is reversed, moving from Layer 1 back to Layer 7. Each layer adds or removes its own header information to ensure proper communication.
The OSI model is a foundational framework for understanding networking concepts and troubleshooting network issues effectively.
