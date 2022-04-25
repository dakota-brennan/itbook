IT VAULT
NETWORK CHAPTER
PHYSICAL LAYER .OVERVIEW

<mark style="background: #D2B3FFA6;">Physical Layer (Layer 1)  </mark> 
#-1_physical_layer

	-nickname
The truck. Moves bits.

	-DEFINITION
<mark style="background: #FFB8EBA6;">This layer</mark> <mark style="background: #FFB86CA6;">deals with</mark> the <mark style="background: #BBFABBA6;">hardware of networks</mark> such as <mark style="background: #BBFABBA6;">cabling</mark>. 
<mark style="background: #FFB8EBA6;">It</mark> <mark style="background: #FFB86CA6;">defines</mark> the <mark style="background: #FFF3A3A6;">mechanical</mark> and <mark style="background: #FFF3A3A6;">electrical standards</mark> of <mark style="background: #BBFABBA6;">interface devices </mark> and <mark style="background: #FFF3A3A6;">the types</mark> of <mark style="background: #BBFABBA6;">cables</mark> <mark style="background: #FFB86CA6;">used to transmit</mark> <mark style="background: #BBFABBA6;">digital signals</mark> (e.g. optical fiber, coaxial cable, wireless etc.)
@ https://www.techopedia.com/definition/24961/osi-protocols Technopedia 

<mark style="background: #FFB8EBA6;">The physical layer</mark> is <mark style="background: #FFB86CA6;">responsible</mark> for the<mark style="background: #FFB86CA6;"> physical cable</mark> or <mark style="background: #FFB86CA6;">wireless connection</mark> between <mark style="background: #BBFABBA6;">network nodes</mark>. 
<mark style="background: #FFB8EBA6;">It</mark> <mark style="background: #FFB86CA6;">defines</mark> the <mark style="background: #BBFABBA6;">connector</mark>, the <mark style="background: #BBFABBA6;">electrical cable</mark> or <mark style="background: #BBFABBA6;">wireless technology</mark> <mark style="background: #FFB86CA6;">connecting</mark> the <mark style="background: #BBFABBA6;">devices</mark>. 
<mark style="background: #FFB8EBA6;">Is</mark> <mark style="background: #FFB86CA6;">responsible</mark> for transmission of the raw data, which is simply a series of 0s and 1s, while taking care of <mark style="background: #FF5582A6;">bit rate control</mark> .
@ https://www.imperva.com/learn/application-security/osi-model/

<mark style="background: #FFB8EBA6;">The physical layer</mark> <mark style="background: #FFB86CA6;">is concerned</mark> with <mark style="background: #FFB86CA6;">transmitting</mark> <mark style="background: #BBFABBA6;">raw bits</mark> <mark style="background: #FFF3A3A6;">over a</mark> <mark style="background: #BBFABBA6;">communication channel</mark>. 
The design issues have to do with making sure that when one side sends a 1 bit, it is received by the other side as a 1 bit, not as a 0 bit. Typical questions are how many volts should be used to represent a 1 and how many for a 0?
how many microseconds a bit lasts?
<mark style="background: #FFF3A3A6;">whether</mark> <mark style="background: #BBFABBA6;">transmission</mark> <mark style="background: #FFF3A3A6;">may proceed simultaneously</mark> in both directions? how the initial connection is established?
and how it is <mark style="background: #FFB86CA6;">torn down</mark> when <mark style="background: #BBFABBA6;">both sides</mark><mark style="background: #FFF3A3A6;"> are finished</mark>?
and <mark style="background: #FFF3A3A6;">how may</mark> <mark style="background: #BBFABBA6;">pins</mark> the <mark style="background: #BBFABBA6;">network connector</mark> <mark style="background: #FFF3A3A6;">has</mark>?
and what each pin is used for?
The <mark style="background: #BBFABBA6;">design issues</mark> <mark style="background: #FFB86CA6;">deal largely with</mark> <mark style="background: #FFF3A3A6;">mechanical</mark>, <mark style="background: #FFF3A3A6;">electrical</mark>, <mark style="background: #FFF3A3A6;">functional</mark>, and <mark style="background: #FFF3A3A6;">procedural</mark> <mark style="background: #BBFABBA6;">interface</mark>.

The physical layer describes:
-Cabling systems as the <mark style="background: #FF5582A6;">transmission media</mark>. 
-Network topology and how the
-<mark style="background: #FF5582A6;">Transmission media</mark> distribution.
I.e. <mark style="background: #FFF3A3A6;">topolgies</mark>: <mark style="background: #BBFABBA6;">bus</mark>, <mark style="background: #BBFABBA6;">star</mark>, and <mark style="background: #BBFABBA6;">ring</mark> 

	-PDU
Bit, symbol

	-FUNCTION
Transmission and reception of raw bit streams over a physical medium
@ https://en.wikipedia.org/wiki/OSI_protocols

#-1_physical_layer/bit_rate_control
#-1_physical_layer/-network_connectors
#-1_physical_layer/transmission_media
#-1_physical_layer/network_topology/-bus
#-1_physical_layer/network_topology-star
#-1_physical_layer/-network_topology/-ring
#-1_physical_layer/-network_topology
#-1_physical_layer/-coaxial_cable
#-1_physical_layer/-wireless
#-1_physical_layer/-optical_fiber