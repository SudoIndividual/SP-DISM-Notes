# Chapter 1
## Basic Functions of a Computer
Computer function can be broken down into three basic task:

 - Input ( e.g recieve instruction from user )
 - Processing ( e.g CPU process instruction from input and send it to the output )
 - Output ( e.g recieve instruction from CPU to perform its task )

![](/Images/1.png)
## Input device
E.g of an input device:
 - Keyboard
- Mouse
- Microphones
- Webcams
- Scanners
## CPU
**CPU** executes instructions from computer programs, such as word processors and from the computer’s operating system.

Current CPUs are composed of processors called **cores**

If there are two or more processors it is called **Multicore**.

**Multicore**:

Multicore CPU enable compter to carry out multiple instruction simultaneously( at the same time )

## Output Device
E.g of an output device:
- Printer
-  Monitor
- Storage device
- network cards
- speakers

## Storage Components

Two main categories of storage:
- Short-term storage ( Volatile )
- Long-term storage ( Non-volatile )

**Volatile**: will lose its content when power is turned off
**Non-Volatile**: maintains it data even when there is no power.
### RAM: Short-term storage:

**Random access memory(RAM)** will lose its content when power is turned off. ( **Volatile** )

RAM have no moving parts and is much faster than access data on a storage

The amount of RAM is important for the computer to function.

If there is not enough RAM to run a program, the computer will use the disk drive to supplement. (**virtual memory**)

#### Virtual memory
- Part of disk storage can be set as virtual memory
- CPU can only access data in RAM
- Less used data are placed in virtual memory
- Data needed by CPU are moved to RAM

![](/Images/2.png)

### Long-Term Storage

**Long-term storage** maintains it data even when there is no power. ( **Non-volatile** )

**Long-term storage** is used to store documents,multimedia files and OS files. ( In short it store files and document )

Amount of storage needed for a computer depend on type and quantity of the file stored.

## Hard drive fundamentals

Magnetic disk called **platters** store data in the form of magnetic pulse

**Actuator arm** have **read/write headers** which used to write data.

## Solid State Drive(SSD)
- SSD is faster and more reliable than hard drives *
- SSD use flash memory *
- SSD have no moving parts *
- SSD has faster access times *
- SSD are more expensive than hard drives *
- SSD most often found in hard drives

## Bus

**Bus** is a collection of wires carrying signals from one place to another on the computer

All data that goes into or comes out of a computer goes through the motherboard

**Type of Bus**:

 - Data Bus
 - Address Bus
 - Control Bus
### Data bus
**Used to carry data signal** from **main memory and CPU vice versa** or from **main memory to input and output devices vice versa**.
### Address Bus
**Used to carry address signals**, eample memory location

### Control Bus

**Used to carry control signals**, exmple read or write from CPU to memory.

### Difference between Address bus and data bus
Data bus carries the data to be stored, while address bus carries the location to where it should be stored.

## Input and out device Polling and interrupt

**Polling:** CPU check input and output device at regular interval whether CPU services is needed.

**Interrupt:** The input and out device interrupt the CPU and request for its services.

## Important Personal Computer Hardwares
Four major PC components:
- Motherboard
- Hard drive
- RAM
- BIOS/CMOS

## BIOS/CMOS Fundamentals

BIOS : basic input output system

1. Set of instructions located in a chip on the motherboard

2. BIOS tells the CPU to perform task like power-on self test( POST ) when power is first applied to the computer.

CMOS:
Configuration of hardware components is store in complementary metal oxides semiconductor (CMOS)

## Computer Boot Procedure
1. Power is applied to the motherboard

2. The CPU starts

3. The CPU carries out the BIOS startup routines,  including the POST

4. Boot devices, as specified in the BIOS configuration, are searched for an OS

5. The OS is loaded into RAM

6. OS services are started

## The Fundamentals of Network Communication

1. A computer network consists of two or more computers connected by some kind of transmission medium
2. Network interface card create and mediate the connection between a computer and network medium
3. MAC address(Media Access Control Address) are unique identifier that is assigned to NIC.
4. SSID are name of the network

## Functional units

###	Primary memory (also called Main memory)
1.	32 bits = 8 bytes
2.	Programs and data must be in the primary memory to be executed


### Cache memory  

1. An adjunct to the main memory, fabricated on the processor chip

2. Much smaller and faster than the main memory

3. Holds sections of the program and data currently/frequently being executed

### Processor
1. Logic circuits for performing arithmetic and logic operations on word-size data operands  

2. Timing and control circuits for fetching program instructions and data from memory, one after another  

3. Registers each of which hold one word of operand data

### Arithmetic and Logic Unit

1. Most computer operations are executed in the ALU of the processor

2. Performs arithmetic or logic operation

### Control Unit
1. Memory, ALU and I/O units store and process information and perform input and output operations
2. The responsibility of the control unit is coordinating the operation of memory,arithmetic and logic unit, and input or output device.

## Computer 

Operation of a computer can be summarized as:

1)Computer accepts information in the form of programs and data through an input unit and stores it in the memory

2)Information stored in the memory is fetched under program control into an ALU, where it is processed

3)Processed information leaves the computer through an output unit

4)All activities in the computer are directed by the Control Unit

### Instruction Cycle
A single cycle of operations (instruction cycle or Machine cycle) consist of:
-	 Fetch
-	Decode
-	Execute
-	Memory Access
-	Write back

### Instructions and Programs: 
1.	Instructions Specifies an operation and location of its data operands 
2.	A 32-bit holds one encoded instruction 
3.	A sequence of instructions executes one after another,constiutes a program
4.	Both a program and data its stored in the main memory

### Instruction Types
1.	Load – Read a data operand from memory or input device into the processor.
2.	Store – write a data operand from a processor register to memory or output device.
3.	Operate – performs arithmetic or logic operations on data operands in processor registers. 

### Processor Components
1.	Program counter register– Holds the memory address of the current instruction 
2.	Instruction Register – Holds the current instruction
3.	General purpose registers - hold data and addresses
4.	Control Circuits and ALU – Fetch and execute instructions 

## Program counter
1. the program counter increases its stored value by 1. After each instruction is fetched, the program counter points to the next instruction in the sequence.

## Handling I/O devices

An application program can:

1. Read data from an input device

2. Write data to an output display screen

3. Sense the readiness of an input or output (I/O) device to perform a transfer

## Performance 

How quickly can a program be executed is determined by:
1. Speed of electronic circuits in the processor
2. Access times to the cache and main memory
3. Design of the instruction set
4. Number of operations that can be done at the same time (Multicore processing)

# Chapter 2

## Arithmetic 

Range: -2^n-1^ to + 2^n-1^-1

Anything above the range is overflow

## Overflow (Addition)
Overflow occurs if:

(+A) + (+B) = −C

(−A) + (−B) = +C

## Overflow (Subtraction)

Overflow occurs if

(+A) − (−B) = −C

(−A) − (+B) = +C

## Signed

For signed integers, the leftmost bit is used to indicate the sign:

- 0  for positive

- 1  for negative

Signed magnitude – Left most bit is not number used as sign (+/-)

1’s complement – flip the bits

2’s complement – flip the bits + add 1 to if number is negative

# Chapter 3

1 k**b**/s = 1000 **bits** per second

1 K**B**/s = 1024 **bytes** per second


Software Components:
-	Network Clients and Server 
-	Network Client Software – Request’s information stored on another network computer. E.g., FTP, Google Chrome
-	Network Server software – Allows a computer to share resources. E.g., Apache Web Server 
-	Protocol – Define rules and formats a computer must use to send information across the network.  (e.g. TCP/IP protocol stack)
-	NIC Drivers – receives data from protocols and forward this data to the physical NIC.

| Step | Description                                                                                                                                             | Layer             |
|------|---------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------|
| 1    | An application tries to access a network resource.                                                                                                      | User application  |
| 2    | Client software detects the attempt to access the network and passes the message on to the network protocol.                                            | Network software  |
| 3    | The protocol packages the message in a format suitable for the network and sends it to the NIC driver.                                                  | Network protocol  |
| 4    | The NIC driver sends the data in the request to the NIC card, which converts it into the necessary signals to be transmitted across the network medium. | Network interface |

## LANs, Internetworks, WANs, and MANs
### LAN

1. Local area network (LAN) – small network, limited to a single collection of machines and connected by one or more interconnecting devices in a small geographic area
### Internetwork

An internetwork is a networked collection of LANs tied together by devices such as routers

Reasons for creation:

- Two or more groups of users and their computers need to be logically separated but still need to communicate

- Number of computers in a single LAN has grown and is no longer efficient

- The distance between two groups of computers exceeds the capabilities of most LAN devices 
### Wide area networks (WANs) 
Wide area networks (WANs) use the services of third-party communication providers to carry network traffic from one location to another

### Metropolitan area networks (MANs)

Metropolitan area networks use WAN technologies to interconnect LANs in a specific geographic region, such as a county of city

### Internet, Intranet, and Extranet

- Internet: a worldwide public internetwork
- Intranet: a private internetwork in which devices and servers are only available to those users connected to the internal network
- Extranet: allows limited and controlled access to internal resources by outside users

## Packets and Frames

Computers transfer information across networks in shorts bursts of about 1500 bytes of data


Reasons data is transferred this way:

 - Pause between bursts allows other computers to transfer data during pauses

 - Allows the receiving computer to process received data

 - Allows the receiving computer receive data from other computers at the same time

 - Gives the sending computer an opportunity to receive data from other computers and perform other processing tasks

 - If an error occurs during transmission of a large file, only the chunks of data involved in the error have to be sent again

### Packet

1. Packet: a chunk of data with a source and destination IP address added to it

### Frame
1. Frame: a packet with the source and destination MAC addresses added to it
2. The process of adding IP addresses and MAC addresses to chunks of data is called encapsulation
3. Information added to the front of the data is called a header and information added to the end is called a trailer(Error-checking)

# Chapter 4

## Repeater and hubs

### Repeater
A repeater receives bit signals generated by NICs and other devices, strengthens them, and then “repeats” them to other parts of the network

### Hub

- Hub is a multiport repeater
- Receives bit signals generated from a connected computer’s NIC on one of its ports
- Cleans the signal by filtering out electrical noise
- Regenerates the signal to full strength
- Transmits the regenerated signal to all other ports where a computer (or other network device) is connected to

## Network switches

–switch actually data in the message, determines which port the destination device is connected to, and forward the message to only that port

### Basic Switch Operation
1. Data is sent onto the medium one frame at a  time
2. Each frame has the destination and source MAC addresses
3. Switch reads the addresses:
- Use the source MAC address of frame to keep a record of which computer is on which port (switching table)
- Forwards the frame to the port where the destination MAC can be found

### Steps of switch operation

1. The switch receives a frame.

2. The switch reads the source and destination MAC addresses.

3. The switch looks up the destination MAC address in its switching table.

4. The switch forwards the frame to the port where the computer owning the MAC address is found.

5. The switching table is updated with the source MAC address and port information.

### Bandwidth

1. Each port gets dedicated bandwidth
- Instead of having to share bandwidth with all ports
2. Multiple conversations can occur simultaneously
3. Can operate in full-duplex mode
- Can send and receive data simultaneously
4. Hubs can only operate in half-duplex mode
- Can send or receive (but not both) at one time
5. Switches are the preferred device because of these advantages

## Access points

1. wireless router is combine of functions of an AP, a switch, and a router

## NIC basics

network interface card (NIC) is used to create and mediate the connection between a computer and the networking medium

1. The tasks a NIC and its driver perform:

- Provide a connection from computer to medium

- Incoming messages: Receives bit signals and assembles them into frames

-- Verifies the destination address

-- Removes frame header and sends the resulting packet to the network protocol

- Outgoing messages: receive packets from network protocol

-- Creates frames by adding MAC addresses/error check

- Converts frame into bit signals suitable for the medium and transmits them
### Mac Address
1. Different NIC card have different mac address
2. MAC address is stored in read-only memory (ROM) on the NIC

### NIC gatekeeper
1. NIC only permits inbound communications if the destination MAC:

- Matches the NICs burned-in address

- Is a broadcast address (ff-ff-ff-ff-ff-ff)

- NIC is in a special mode called promiscuous

2. Promiscuous mode allows the NIC to process all frames it sees

### NIC Indicator Lights
1. amber for 100 Mbps and green for 1000 Mbps

## Routers

1. The following are the differences between routers and switches

 - Routers connect LANs, switches connect computers to form LANs

 - Routers work with logical (IP) addresses, switches work with physical (MAC) addresses

 - Routers work with packets, switches with frames

 - Routers don’t forward broadcasts, switches do

 - Routers use routing tables, switches use switching tables

## Routers Work with IP Addresses and Routing Tables

 - Default route — where to send a packet when the router doesn’t have an entry in its routing table

 - Network unreachable — Message sent when the network can’t be found and no default route

 - Default gateway — In a computer’s IP address configuration – the IP address of the computer’s router
