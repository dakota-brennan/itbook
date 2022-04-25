IT VAULT
NETWORK
OSI Overview

![](IEB90_p38_1.jpg)

Open Systems Interconnection − a network model including protocols developed by an ISO standards committee with the intent to standardize network communications. From Linux Guide @FirstLinux
@ "Linux dictionary" p. 1152

Advantage of using the OSI model as a reference point lies in its layered approach:
"The layered approach offers several advantages. By separating networking functions into logical smaller pieces, network problems can more easily be solved through a divide-and-conquer methodology. OSI layers also allow extensibility. New protocols and other network services are generally easier to add to a layered architecture."
@

The OSI model consists of 7 layers:
<mark style="background: #ABF7F7A6;">Application, Presentation, Session</mark> 
These "layers comprise the upper layers of the OSI Model. Software in these layers performs application specific functions like data
formatting, encryption, and connection management."
@

<mark style="background: #ABF7F7A6;">Transport, Network, Data Link, Physical</mark> 
Provide the network foundation 
"The transport, network, data link,
and physical layers comprise the lower layers, which provide more primitive network specific functions like routing, addressing, and flow controls."
@

"The seven OSI layers are defines as follows (Feig)1:
7. Application: Provides different services to the application
6. Presentation: Converts the information
5. Session: Handles problems which are not communication issues
4. Transport: Provides end to end communication control
3. Network: Routes the information in the network
2. Data Link: Provides error control
1. Physical: Connects the entity to the transmission media
(An acronym used to help remember the model from bottom to top is “Please Do Not Throw Sausage Pizza Away.” From top down the “All People Seem To Need Data Processing” acronym can be utilized.)"
@

<mark style="background: #ABF7F7A6;">Application Layer (L 7)</mark> 
The application layer is the top layer of the OSI model. It provides a set of interfaces for applications to obtain access to networked services as well as access to network services that support applications directly. This layer also provides application access security checking and information validation. The Application Layer provides the following functions (Tan Ten Hong)3:

·  <mark style="background: #FFB8EBA6;">File-Transfer-Access-and-Management (FTAM)</mark> : Provides handling services in the network. This includes the movement of files between different systems, reading, writing and deletion of remote files, and management of remote file storage.

·  <mark style="background: #FFB8EBA6;">Virtual_Terminal (VT)</mark> : Provides services to access applications in different remote computer systems through stimulating a real terminal.

·  <mark style="background: #FFB8EBA6;">Electronic-Mail-and-Messaging-Handling (MHS)</mark> : Facilitates the electronic exchange of documents.

·  <mark style="background: #FFB8EBA6;">Directory-Services (DS)</mark> : Provides services with the ability to match names with addressing information.

·  <mark style="background: #FFB8EBA6;">Common-management-Information-Protocol (CMIP)</mark> : Provides services for network management.

	protocol
HTTP
SMTP
etc.

	protocol data unit
Messages

	addressing
N/A

	specialist function

Tags:
#-7_application_layer/-directory_service
#-7_application_layer/-virtual-technolog
#-7_application_layer/-Electronic-Mail-and-Messaging-Handling
#-7_application_layer/-File_Transfer_Access_and_Management
#-7_application_layer/Common-management-information-protocol

<mark style="background: #ABF7F7A6;">Presentation Layer (L 6)</mark> 
The presentation layer is responsible for the format of the data transferred during
network communications. This layer is concerned with the syntax and semantics of the information transmitted. For outgoing messages, it converts data into a generic format for the transmission. For the incoming messages, it converts the data from the generic form to a format understandable to the receiving application. Different computers have different codes for representing data. The presentation layer makes it possible for computers with different representation to communicate. The presentation layer provides common communication services such as encryption, text compression, and reformatting.
The presentation layer is also concerned with other aspects of information
representation. Data compression can be used to reduce the number of bits that havex
to be transmitted. Cryptography is frequently required for privacy and authentication.

	protocol


	protocol data unit


	addressing


	specialist function
	

<mark style="background: #ABF7F7A6;">Session Layer (L 5)</mark> 
The session layer permits two parties to hold ongoing communications called a session across a network. The applications on either end of the session can exchange data or
send packets to another for as long as the session lasts. The session layer handles
session setup, data or message exchanges, and tear down when the session ends. It
also monitors session identification so only designated parties can participate and
security services to control access to session information. A session can be used to
allow a user to log into a remote time-sharing system or transfer a file between two
machines. (Tan Ten Hong)3
The session layer has the option of providing one-or-two-way communication called
dialogue control. Sessions can allow traffic to go in both directions at the same time, or
in only one direction at a time. Token management may be used to prevent both sides
from attempting the same operation at the same time. To manage these activities, the
session layer provides tokens that can be exchanged. Only the side holding the token
is permitted to perform the critical operation.
Another session service is synchronization. Consider the problems that occur when
transferring a file between two machines and the system crashes not being able to
complete the transfer. This process must be restarted from the beginning. To avoid
this problem, the session layer provides a way to insert checkpoints into the data
stream, so that after a crash, only the data after the last checkpoint has to be repeated.

	protocol


	protocol data unit


	addressing


	specialist function


<mark style="background: #ABF7F7A6;">Transport Layer (L 4)</mark> 
The basic function of the transport layer is to accept data from the session layer, split it up into smaller units, pass it to the network layer, and ensure that the bits delivered are the same as the bits transmitted without modification, loss or duplication.
If an error occurs during transmission, the transport layer must correct it. There is a set of rules to follow that detail the handling of the error and how to correct it. The
correction may mean re-sending just the damaged data or restarting from the beginning.
This can be achieved because the transport layer protocol includes the capability to
acknowledge the receipt of a packet. “If no acknowledgement is received, the transport
layer can retransmit the packet or time-out the connection and signal an error. The
transport protocol can also mark packets with sequencing information so that the
destination system can properly order the packets if they are received out of order.”
(Tan Ten Hong)3
If the transport connection requires a high throughput, the transport layer might create multiple network connection by dividing the data among the network connections to improve the throughput. However, the transport layer might multiplex several transport connections onto the same network to reduce costs. This multiplexing is transparent to the session layer.
“Transport protocols provide the capability for multiple application processes to access the network by using individual local addresses to determine the destination process for each data stream. These addresses are often referred to as ports and connection opened to these ports as sockets.” (Tan Ten Hong)3

	protocol
TCP/UDP

	protocol data unit
Segment

	addressing
Port #

	specialist function


<mark style="background: #ABF7F7A6;">Network Layer (L 3)</mark> 
The network layer controls the operation of a sub-net, provides routing, congestion
control and accounting. The network layer provides both connectionless and
connection-oriented services. A key design issue is determining how packets are
routed from source to destination. Routes can be based on static tables that are within
the network and rarely change. They could also be determined at the start of each
conversion. Finally, they could be highly dynamic, being newly determined for each
packet to reflect the current network load. It is up to the network layer to allow
heterogeneous networks to be interconnected. The IP protocol resides in this layer. All
routers in the network are operating at this level.
If too many packets are present in the sub-net at the same time, bottlenecks will form.
The network layer helps to control this congestion. An accounting function is built into the network layer to ensure that the number of bits sent is the number of bits received.
Controls over network connections, logical channels, segmenting and sequencing, and
data flow can be placed in this layer.

	protocol
IP

	protocol data unit
Datagram

	addressing
IP address

	specialist function


<mark style="background: #ABF7F7A6;">Data Link Layer (L 2)</mark> 

This layer describes technology that is responsible for making data from L1 universally accessible on all other layers, regardless of which physical method is in use. 
The main task of the data link layer is to take a raw transmission and transform it into a line that appears free of transmission errors in the network layer. It accomplishes this task by having the sender break the input data up into data frames, transmit the frames sequentially, and process the acknowledgment frames sent back by the receiver. The protocol packages the data into frames that contain source and destination addresses.
These frames refer to the physical hardware address of each network card attached to
the network cable. Ethernet, Token Ring, and ARCnet are examples of LAN data link
protocols. If communication extends beyond the LAN onto the Internet, the network
might use other <mark style="background: #FFB86CA6;">data link protocols</mark> , such as Point-to-Point Protocol (PPP) or Serial Line Internet Protocol (SLIP).
The data link layer sends blocks of data with the necessary synchronization, bit error
detection/correction error control, and flow control. This control of data flow controls
approximately 70 percent of all error handling. Since the physical layer merely accepts
and transmits a stream of bits without any regard to the meaning of the structure, it is up to the data link layer to create and recognize frame boundaries. This can be
accomplished by attaching special bit patterns to the beginning and end of the frame.
<mark style="background: #FFB86CA6;">Encryption</mark> can be used to protect the message as it flows between each network node. Each node then decrypts the message received and re-encrypts it for transmission to
the next node.

	protocol
Ethernet
Wi-fi

	protocol data unit
Frames

	addressing
MAC address

	specialist function
	

<mark style="background: #ABF7F7A6;">Physical Layer (L 1)</mark> 
L1 is responsible for describing the method of data transmission and the technology it uses.

	Method
Transmitting raw bits over a communication channel, via Moduling (also known as <mark style="background: #FFB86CA6;">Line Coding</mark>) it is the modulation of an electrical charge so that each side of a connection knows what is a one and what is a zero. The design issues have to do with making sure that when one side sends a 1 bit, it is received by the other side as a 1 bit, not as a 0 bit. Typical questions are how many volts should be used to represent a 1 and how many for a 0, how many microseconds a bit lasts, whether transmission may proceed simultaneously in both directions, how the initial connection is established and how it is torn down when both sides are finished (aka <mark style="background: #FFB86CA6;">Topologies</mark> ) and how may pins the network connector has and what each pin is used for. The design issues deal largely with mechanical, electrical, functional, and procedural interface.
There are three types of communication:
    -Simplex (one way across the cable)
    -Duplex (simultaneous)
    -Half-duplex (direction by turns, only one device speaks)

	Technology
 Device that transmit data
	The physical layer describes cabling systems as the transmission media.
	This is <mark style="background: #FFB86CA6;">Ethernet over Twisted Pair Technologies</mark> 
	https://en.wikipedia.org/wiki/Ethernet_over_twisted_pair


![](1920px-Twisted_pair_based_ethernet.svg.png)
The cable ends with a plug (RJ45 most common RJ - registered jack). 
Goes into computers, servers and patches. 
A patch may be considered a socket station which directs the signal through wall cables to its destination. 

	
	topologies
Bus
Star
Ring

	protocol
10 Base T
802.11

	protocol data unit
Bits

	addressing
N/A

	form
Cables
- pair of twisted cables (they are twisted for the purpose of eliminating electromagnetic interference and crosstalk from neighboring pairs)
- hubs

specialist function
	
Network setup
Troubleshooting


<mark style="background: #ABF7F7A6;">Concepts</mark> 
Three concepts are central to the OSI model:
1. Services
2. Interfaces
3. Protocols
Information from each layer passes up to the next layer, so that a protocol operating at
a given layer can access all the information the protocols below it collect or prepare.
Each layer performs some services for the layer above it. The service definition tells
what the layer does, not how entities above it access or how the layer works. A layer’s
interface tells the processes above it how to access it. It specifies what the parameters
are and what results to expect. The layer can use any protocols as long as it provides
the offered services.


LINK LIST:
