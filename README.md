# A Simple TCP Finite State Machine Model
A simple TCP FSM using a dictionary.

# What is a Finite State Machine (FSM)?
A Finite State Machine, or FSM, is a computational model used to simulate sequential logic, or in simpler terms, to represent workflows. 
It’s called a ‘machine’ because it transitions from one ‘state’ to another based on input and the current state. 
The number of states is finite, hence the name ‘Finite State Machine’.

FSMs are widely used in computer science and engineering for modeling systems’ behavior, designing hardware digital systems, game development, algorithms, and more. 
They are perfect for situations where we have a limited number of states, and the system can only be in one state at any given time.

# What is Transmission Control Protocol (TCP)?
Transmission Control Protocol (TCP) is one of the main protocols in the Internet protocol suite. 
It’s a set of rules that governs the delivery of data over the Internet or local network. 
It’s a connection-oriented protocol, which means a connection is established and maintained until the application programs at each end finish exchanging messages.

TCP provides reliable, ordered, and error-checked delivery of a stream of bytes between applications running on hosts communicating via an IP network. 
It’s used by major internet applications such as the World Wide Web, email, remote administration, and file transfer.

# Modeling TCP with FSM
TCP states can be modeled effectively using an FSM. Each state represents a particular condition in the communication process, 
like waiting for a connection or data transfer. 
The transitions between these states are triggered by events or conditions, such as the receipt of a data packet.

For example, when a TCP connection is established, it starts in the ‘CLOSED’ state. 
When the application on the local machine calls for a connection to be established (APP_ACTIVE_OPEN event), 
the state changes to ‘SYN_SENT’. This is an example of a state transition in the TCP FSM.
