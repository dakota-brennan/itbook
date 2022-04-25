IT VAULT
NETWORK CHAPTER
TRIVIAL FILE TRANSFER PROTOCOL

#-7_application_layer/TFTP

TFTP stands for <mark style="background: #FFB86CA6;">Trivial File Transfer Protocol</mark> its used for sending a file from the server to the client. TFTP uses the <mark style="background: #FF5582A6;">concept of UDP</mark> <mark style="background: #FFF3A3A6;">to share files</mark> between <mark style="background: #FFF3A3A6;">server</mark> and <mark style="background: #FFF3A3A6;">client</mark>. Here UDP stands for <mark style="background: #FF5582A6;">User Datagram Protocol</mark>. 
It is generally used for communicating files among machines set up in the local intranet only. 
TFTPs most important feature is that it <mark style="background: #FFF3A3A6;">uses a minimal amount of memory</mark>. 
This application layer Protocol <mark style="background: #FFF3A3A6;">could be used to communicate boot files if computers do not have hard disks</mark> . 
It generally uses <mark style="background: #ADCCFFA6;">port 69</mark>; however, the port used for communication could be defined by when TFTP is being set up.
@ https://www.educba.com/application-layer-protocols/

TFTP is the stripped-down, stock version of FTP, but it’s the protocol of choice if you know exactly what you want and where to find it. It’s a technology for transferring files between network devices and is a simplified version of FTP.<mark style="background: #ADCCFFA6;"> Port 69</mark> 

#-7_application_layer/TFTP/port_69


	COMMAND

tftp [ options... ] [host [port]] [-c command]


!!!! - in this case when should this protocol be used?

@ https://www.geeksforgeeks.org/protocols-application-layer/