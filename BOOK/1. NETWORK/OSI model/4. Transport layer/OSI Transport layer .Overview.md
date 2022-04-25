IT VAULT
NETWORK CHAPTER
OSI TRANSPORT LAYER

<mark style="background: #ABF7F7A6;">Transport layer(L 4)</mark> 

#-4_transport_layer

	-nickname
Middle manager. Segment ID/assembly.

	-DEFINITION
The transport layer takes data transferred in the session layer and breaks it into “segments” on the transmitting end. It is responsible for reassembling the segments on the receiving end, turning it back into data that can be used by the session layer. The transport layer carries out flow control, sending data at a rate that matches the connection speed of the receiving device, and error control, checking if data was received incorrectly and if not, requesting it again.
@ https://www.imperva.com/learn/application-security/osi-model/

The basic function of the transport layer is to accept data from the session layer, split it up into smaller units, pass it to the network layer, and ensure that the bits delivered are the same as the bits transmitted without modification, loss or duplication.
If an error occurs during transmission, the transport layer must correct it. There is a set of rules to follow that detail the handling of the error and how to correct it. The correction may mean re-sending just the damaged data or restarting from the beginning.
This can be achieved because the transport layer protocol includes the capability to acknowledge the receipt of a packet. “If no acknowledgement is received, the transport layer can retransmit the packet or time-out the connection and signal an error. The transport protocol can also mark packets with sequencing information so that the
destination system can properly order the packets if they are received out of order.”
(Tan Ten Hong)3

If the transport connection requires a high throughput, the transport layer might create multiple network connection by dividing the data among the network connections to improve the throughput. However, the transport layer might multiplex several transport connections onto the same network to reduce costs. This multiplexing is transparent to the session layer.
“Transport protocols provide the capability for multiple application processes to access the network by using individual local addresses to determine the destination process for each data stream. These addresses are often referred to as ports and connection opened to these ports as sockets.” (Tan Ten Hong)3

	-PDU
Segment, Datagram

	-FUNCTION
Reliable transmission of data segments between points on a network, including [segmentation](https://en.wikipedia.org/wiki/Packet_segmentation "Packet segmentation"), [acknowledgement](https://en.wikipedia.org/wiki/Acknowledgement_(data_networks) "Acknowledgement (data networks)") and [multiplexing](https://en.wikipedia.org/wiki/Multiplexing "Multiplexing")
@ https://en.wikipedia.org/wiki/OSI_protocols

LINK LIST
