IT VAULT
NETWORK CHAPTER
OSI APPLICATION LAYER
FILE TRANSFER PROTOCOL

#-7_application_layer/FTP

FTP stands for File Transfer Protocol. It is a application layer protocol that is used for transforming a file from one location to another, i.e. from one host to another host. 
It is a standard mechanism that is provided by <mark style="background: #FF5582A6;">TCP/IP</mark> . 
Transferring files from one system to another seems very simple, but some problems need to be dealt with before transforming files. 

It uses TCP services. It needs two TCP connections. One is a <mark style="background: #FF5582A6;">Control connection</mark> , and another is a <mark style="background: #FF5582A6;">Data connection</mark> . For control connection, it uses well-known <mark style="background: #ADCCFFA6;">port 21</mark> , and for data connection, it uses well-known <mark style="background: #ADCCFFA6;">port 20</mark> .
@ https://www.educba.com/application-layer-protocols/

!!!! - but some problems need to be dealt with before transferring files (what problems need to be dealt with?)

FTP stands for <mark style="background: #BBFABBA6;">file transfer protocol</mark>. It is the protocol that actually lets us transfer files. It can facilitate this between any two machines using it. But FTP is not just a protocol but it is also a program. FTP promotes sharing of files via <mark style="background: #FF5582A6;">remote computers</mark> with reliable and efficient data transfer.  <mark style="background: #ADCCFFA6;">port 20</mark> for data and <mark style="background: #ADCCFFA6;">port 21</mark> for control.
#-7_application_layer/FTP/port_20
#-7_application_layer/FTP/port_21

	command
ftp machinename

@ https://www.geeksforgeeks.org/protocols-application-layer/