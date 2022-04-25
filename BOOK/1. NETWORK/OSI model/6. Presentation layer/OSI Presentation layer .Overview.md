IT VAULT
NETWORK CHAPTER
OSI PRESENTATION LAYER

<mark style="background: #ABF7F7A6;">Presentation Layer (Layer 6)</mark> 

#-6_presentation_layer

	Definition
The presentation layer prepares data for the application layer. It defines how two devices should encode, encrypt, and compress data so it is received correctly on the other end. The presentation layer takes any data transmitted by the application layer and prepares it for transmission over the session layer.
@ https://www.imperva.com/learn/application-security/osi-model/

The presentation layer is responsible for the format of the data transferred during
network communications. 
This layer is concerned with the syntax and semantics of the information transmitted. For outgoing messages, it converts data into a generic format for the transmission. For the incoming messages, it converts the data from the generic form to a format understandable to the receiving application. 
Different computers have different codes for representing data. The presentation layer makes it possible for computers with different representation to communicate. 
The presentation layer provides common communication services such as:
- encryption
- text compression
- reformatting

The presentation layer is also concerned with other aspects of information
representation. Data compression can be used to reduce the number of bits that have
to be transmitted. Cryptography is frequently required for privacy and authentication.
@543

	-PDU
Data

	-FUNCTION
Translation of data between a networking service and an application; including [character encoding](https://en.wikipedia.org/wiki/Character_encoding "Character encoding"), [data compression](https://en.wikipedia.org/wiki/Data_compression "Data compression") and [encryption/decryption](https://en.wikipedia.org/wiki/Encryption "Encryption")
@ https://en.wikipedia.org/wiki/OSI_protocols


	LINK LIST
