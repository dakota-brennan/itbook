IT VAULT
NETWORK CHAPTER
OSI DATA LINK LAYER

<mark style="background: #D2B3FFA6;">Data Link Layer (Layer 2) </mark> 
#-2_data_link_layer/logical_link_control_sublayer 
#-2_data_link_layer/media_access_control_sublayer

	-nickname
Envelope shuffler. Organizes bits into frames.

The <mark style="background: #FFB8EBA6;">data link layer</mark> <mark style="background: #FFB86CA6;">establishes</mark> and <mark style="background: #FFB86CA6;">terminates</mark> a <mark style="background: #FFF3A3A6;">connection</mark> between<mark style="background: #BBFABBA6;"> two</mark> physically-connected <mark style="background: #BBFABBA6;">nodes</mark> on a <mark style="background: #BBFABBA6;">network</mark>.
<mark style="background: #FFB8EBA6;">It</mark> <mark style="background: #FFB86CA6;">breaks up</mark> <mark style="background: #BBFABBA6;">packets</mark> into <mark style="background: #BBFABBA6;">frames</mark> and <mark style="background: #FFB86CA6;">sends</mark> them from <mark style="background: #FFF3A3A6;">source</mark> to <mark style="background: #FFF3A3A6;">destination</mark>.

This layer is composed of two sublayers: 
1) <mark style="background: #FFB8EBA6;">Logical Link Control (LLC)</mark>, which<mark style="background: #FFB86CA6;"> identifies</mark> <mark style="background: #FFB8EBA6;">network protocols</mark>, <mark style="background: #FFB86CA6;">performs</mark> <mark style="background: #FFB8EBA6;">error checking</mark> and <mark style="background: #FFB8EBA6;">frame synchronization</mark>. 
2) <mark style="background: #FFB8EBA6;">Media Access Control (MAC)</mark> which uses the <mark style="background: #FFB8EBA6;">MAC address</mark> <mark style="background: #FFB86CA6;">to connect</mark> <mark style="background: #BBFABBA6;">devices</mark> and <mark style="background: #FFB86CA6;">define</mark> <mark style="background: #BBFABBA6;">permissions</mark> to <mark style="background: #FFB86CA6;">transmit</mark> and <mark style="background: #FFB86CA6;">receive</mark> <mark style="background: #BBFABBA6;">data</mark>.
@ https://www.imperva.com/learn/application-security/osi-model/

The <mark style="background: #FFF3A3A6;">main task</mark> of the <mark style="background: #FFB8EBA6;">data link layer</mark> is to take a <mark style="background: #FFF3A3A6;">raw transmission</mark> and <mark style="background: #FFF3A3A6;">transform</mark> it <mark style="background: #FFF3A3A6;">into a line</mark> that appears free of <mark style="background: #FFB8EBA6;">transmission errors</mark> in the network_layer . It accomplishes this task <mark style="background: #FFF3A3A6;">by</mark> having the <mark style="background: #BBFABBA6;">sender</mark> <mark style="background: #FFF3A3A6;">break</mark> the <mark style="background: #BBFABBA6;">input data</mark> up into <mark style="background: #BBFABBA6;">data frames</mark>, <mark style="background: #FFF3A3A6;">transmit</mark> the frames <mark style="background: #FFF3A3A6;">sequentially</mark>, and <mark style="background: #FFF3A3A6;">process</mark> the <mark style="background: #FFF3A3A6;">acknowledgment frames</mark> sent back by the <mark style="background: #BBFABBA6;">receiver</mark> . The protocol packages the data into frames that contain source and destination addresses.
These frames refer to the physical hardware address of each network card attached to the network cable. <mark style="background: #FFB8EBA6;">Ethernet</mark>, <mark style="background: #FFB8EBA6;">Token Ring</mark>, and <mark style="background: #FFB8EBA6;">ARCnet</mark> are examples of LAN data link protocols. If communication extends beyond the LAN onto the Internet, the network might use other data link protocols, such as <mark style="background: #FFB8EBA6;">Point-to-Point-Protocol (PPP)</mark> or <mark style="background: #FFB8EBA6;">Serial-Line-Internet-Protocol (SLIP)</mark>.

The <mark style="background: #FFB8EBA6;">data link layer</mark> <mark style="background: #FFB86CA6;">sends</mark> <mark style="background: #BBFABBA6;">blocks</mark> of <mark style="background: #BBFABBA6;">data</mark> with the necessary synchronization, bit error detection/correction error control, and flow control. This control of data flow controls approximately 70 percent of all error handling. Since the physical layer merely accepts and transmits a stream of bits without any regard to the meaning of the structure, it is upto the data link layer to create and recognize frame boundaries. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.

Encryption can be used to protect the message as it flows between each network node.
Each node then decrypts the message received and re-encrypts it for transmission to
the next node.

	-PDU
Frame 

	-FUNCTION
Reliable transmission of data frames between two nodes connected by a physical layer


LINK LIST


#-2_data_link_layer/ARCnet
#-2_data_link_layer/data_frames
#-2_data_link_layer/error_checking
#-2_data_link_layer/ethernet
#-2_data_link_layer/frame_synchronisation
#-2_data_link_layer/MAC_address
#-2_data_link_layer/network_protocols
#-2_data_link_layer/PPP 
#-2_data_link_layer/SLIP
#-2_data_link_layer/Token_ring
#-2_data_link_layer/-4_transmission_layer
