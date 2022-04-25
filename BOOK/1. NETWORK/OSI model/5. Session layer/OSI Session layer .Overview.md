IT VAULT
NETWORK CHAPTER
OSI SESSION LAYER

<mark style="background: #ABF7F7A6;">Session Layer (Layer 5)</mark> 

#-5_session_layer

	-nickname
Negotiator. Establishes, manages and ends sessions.

	-DEFINITION
The session layer creates <mark style="background: #FF5582A6;">communication channels</mark> , called <mark style="background: #FF5582A6;">sessions</mark> , between devices. It is responsible for opening sessions, ensuring they remain open and functional while data is being transferred, and closing them when communication ends. The session layer can also set <mark style="background: #FF5582A6;">checkpoints</mark> during a data transfer—if the session is <mark style="background: #FFF3A3A6;">interrupted</mark> , devices can <mark style="background: #FFF3A3A6;">resume data transfer </mark> from the <mark style="background: #FFF3A3A6;">last checkpoint</mark> .
@ https://www.imperva.com/learn/application-security/osi-model/

	-function
The session layer permits two parties to hold ongoing communications called a session
across a network. The <mark style="background: #FFF3A3A6;">applications</mark> on either end of the session <mark style="background: #FFF3A3A6;">can exchange data</mark> or
<mark style="background: #FFF3A3A6;">send packets</mark> to another for <mark style="background: #FFF3A3A6;">as long as the session lasts</mark> . The session layer handles:
- session setup
- data or message exchanges
- tear down when the session ends. 
- monitors <mark style="background: #FF5582A6;">session identification</mark> (so <mark style="background: #FFF3A3A6;">only</mark> designated parties can participate)
- monitors <mark style="background: #FF5582A6;">security services</mark> (to <mark style="background: #FFF3A3A6;">control access</mark> to session information). 
- allows a <mark style="background: #FFF3A3A6;">user</mark> to <mark style="background: #FFF3A3A6;">log into</mark> a <mark style="background: #FF5582A6;">remote time-sharing system</mark> 
- allows <mark style="background: #FF5582A6;">file transfer</mark> between two machines. (Tan Ten Hong)3

		-dialog control
The session layer has the option of providing one-or-two-way communication called
<mark style="background: #FF5582A6;">dialogue control</mark> . Sessions can <mark style="background: #FFF3A3A6;">allow traffic</mark> to go in <mark style="background: #FFF3A3A6;">both directions</mark> at the same time, <mark style="background: #FFF3A3A6;">or</mark> in only <mark style="background: #FFF3A3A6;">one direction</mark> at a time. <mark style="background: #FF5582A6;">Token management</mark> may be used to <mark style="background: #FFF3A3A6;">prevent</mark> both sides from <mark style="background: #FFF3A3A6;">attempting</mark> the <mark style="background: #FFF3A3A6;">same operation</mark> at the <mark style="background: #FFF3A3A6;">same time</mark> . To manage these activities, the session layer <mark style="background: #FFF3A3A6;">provides tokens</mark> that can be <mark style="background: #FFF3A3A6;">exchanged</mark> . Only the side holding the token is <mark style="background: #FFF3A3A6;">permitted to perform</mark> the critical <mark style="background: #FFF3A3A6;">operation</mark> .

	-synchronisation
Another session service is <mark style="background: #FF5582A6;">synchronization</mark> . Consider the problems that occur when
<mark style="background: #FFF3A3A6;">transferring a file</mark> between two machines and the <mark style="background: #FFF3A3A6;">system crashes</mark> not being able to
complete the transfer. This <mark style="background: #FFF3A3A6;">process must be restarted</mark> from the beginning. <mark style="background: #FFF3A3A6;">To avoid</mark> 
this problem, the session layer provides a way to <mark style="background: #FFF3A3A6;">insert checkpoints</mark> into the <mark style="background: #FFF3A3A6;">data
stream</mark> , so that after a crash, only the <mark style="background: #FFF3A3A6;">data after the last checkpoint</mark> has to be <mark style="background: #FFF3A3A6;">repeated</mark> .

	-PDU
Data

	-FUNCTION
Managing communication [sessions](https://en.wikipedia.org/wiki/Session_(computer_science) "Session (computer science)"), i.e., continuous exchange of information in the form of multiple back-and-forth transmissions between two nodes
@ https://en.wikipedia.org/wiki/OSI_protocols

LINK LIST
