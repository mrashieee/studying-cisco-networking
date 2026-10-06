# Communication Principles

## Communication Protocols

Even in real life communication takes place in different
protocols. There are rules that govern the conversation which also
includes the environment and reason for the conversation. That's why
you don't talk to interviewers like how you do casually with your
friend. The rules or agreements to govern the communication we
establish are:

- **Method**: Before communicating we have to agree on the way or
  method of communication that everyone participating can perceive.

- **Language**: We have to decide on the language we are using in
  communication that all participants can understand.

- **Confirmation**: Communication can only be successful when both
  recipient and sender confirm/understand.

Network communications use the human conversation fundamentals like:

- An identified sender and receiver.  
- Agreed upon method of communicating.  
- Common language and grammar.  
- Speed and timing of delivery.  
- Confirmation or acknowledgment requirements.  

## Why Protocols Matter

Just like humans, computers use rules (or protocols) in order to
communicate. Protocols are required for computers to properly
communicate across the network. In both a wired and wireless
environment, a local network is defined as an area where all hosts
must "speak the same language", in computer terms it means they must
"share a common protocol".

Networking protocol characteristics define many aspects of
communication over the local network:

- **Message format**: When a message is sent, it must use a specific
  format or structure. Message formats depend on the type of message
  and channel that is used to deliver the message.

- **Message Size**: The rules that govern the size of the pieces
  communicated across the network are very strict. They can be
  different, depending on the channel used. When a long message is
  sent from one host to another over a network, it may be necessary to
  break the message into smaller pieces in order to ensure that the
  message can be delivered reliably.

- **Timing**: Network communication functions mostly depend on
  timing. Timing determines the speed, both sides must agree on how
  fast bits fly past. Too fast or slow can make the receiver read
  garbage. (it's like talking too fast won't be good for the other
  person to understand what you are saying.) Also on a shared network
  shouting at once will cause collision.

- **Encoding**: Bits get converted into signal patterns for the
  medium. The receiving side knows how to decode because both sides
  follow the same standard.

- **Encapsulation**: It is the process of adding information to the
  pieces of data that make up the message. The information includes
  addressing information that identifies the source and destination
  hosts. Otherwise it cannot be delivered. In addition to addressing
  there may be other information in the header that ensures that the
  message is delivered to the correct application on the destination
  host.

- **Message pattern**: the rule for whether a message needs
  an answer back. Acknowledged pattern waits for confirmation
  before sending the next. Streamed pattern just keeps sending
  without checking, which is fast but some data might never
  arrive.

## Communication Standards

### Internet Standard

A standard is a set of rules that determines how something must be
done. Because of these standards and protocols, different types of
devices send and receive data to each other over the network with no
extra setup. That's why, even if one person sends an email via a
personal computer, another person can use a mobile phone to receive
and read the email as long as the mobile phone uses the same standards
as the personal computer.

## Standards Organizations

Internet standards come from open discussion, testing, and agreement
between many organizations. Every step of a new standard gets written up
as a numbered Request for Comments (RFC) so its history is
tracked. The IETF (Internet Engineering Task Force) publishes and
manages those RFCs.

## Network Communication Models

### TCP/IP Model

Transmission Control Protocol / Internet Protocol is a layered model
which helps us visualize how the various protocols work together to
enable network communication. The first layered model for internetwork
communications was created in the early 1970s and is referred to as
the internet model which defines the four categories of functions
that must occur in order for successful communications. The suite of
TCP/IP protocols follows the structure of this model. Because of this
the internet model is commonly referred to as the TCP/IP model.

Layering helps because:
- Each layer has defined info to act on and a set interface to the
  layers above and below, which makes designing protocols easier.
- Products from different makers can work together.
- One layer can change without touching the others.
- It gives everyone common words to describe networking with.

| TCP/IP Layer       | Description                                                             |
|:-------------------|:------------------------------------------------------------------------|
| 4 - Application    | Represents data to the user, plus encoding and dialog control.          |
| 3 - Transport      | Supports communication between various devices across diverse networks. |
| 2 - Internet       | Determines the best path through the network.                           |
| 1 - Network Access | Controls the hardware devices and media that make up the network.       |

### The OSI Reference Model


Two kinds of models exist:

- **Protocol model**: matches one real protocol suite. It describes
  what each layer of that suite actually does, since the suite's
  protocols were built to provide everything needed to communicate.
  TCP/IP is a protocol model.

- **Reference model**: only lists the functions each layer must get
  done, without saying how to do them. Not detailed enough to build
  from - its job is making the functions and processes clear so
  networks can be designed, specified, and troubleshot.

The famous reference model is OSI (Open Systems Interconnection), made
by the ISO (International Organization for Standardization). Seven
layers, used for designing networks, writing specs, and
troubleshooting.

| OSI Layer        | Description                                                               |
|:-----------------|:--------------------------------------------------------------------------|
| 7 - Application  | Protocols for process-to-process<br>communication.                        |
| 6 - Presentation | Common representation of data<br>between application services.            |
| 5 - Session      | Organizes dialogue and manages<br>data exchange.                          |
| 4 - Transport    | Segments, transfers, and reassembles<br>data between end devices.         |
| 3 - Network      | Exchanges data pieces between<br>identified end devices.                  |
| 2 - Data Link    | Methods for exchanging frames<br>over common media.                       |
| 1 - Physical     | Mechanical, electrical, and procedural<br>means for physical connections. |

## OSI and TCP/IP Model Comparison

The TCP/IP model is a method for visualizing the interactions between
different protocols, it does not describe how general functions that
are necessary for all networking communications. It only describes the
networking functions specific to those protocols in use in the TCP/IP
protocol suite. OSI layers describe them more indepth of what all
protocols are used. Because of this transport and network layers are
contained as transport and internet layers in TCP/IP model, but the
network access and application layers from TCP/IP are further divided
in the OSI model to describe the discrete functions that occur in
these layers.

```
OSI (7 layers)              TCP/IP (4 layers)
==================          ==================
 7 - Application        \
 6 - Presentation        +-->  Application
 5 - Session            /
 4 - Transport          -->  Transport
 3 - Network            -->  Internet
 2 - Data Link          \
 1 - Physical            +-->  Network Access
```

- **Application layer split**: TCP/IP has one application layer
  doing the work of OSI's top three. Session keeps the conversation
  going between the two ends. Presentation handles formats and
  disguises like encryption. Application is the protocols your
  programs speak, like HTTP and DNS. The split is just a guide
  for developers writing apps that talk over networks.

- **Middle layers match**: OSI's network layer and TCP/IP's
  internet layer do the same job (getting packets to the right
  address), and both transport layers do the same job (delivering
  them in order, resending lost ones).

- **Network Access layer split**: TCP/IP bundles wires and frames into
  one Network Access layer. OSI keeps them as two. Physical is the
  network media itself - unplugged cable, dead port, no signal at
  all. Data Link is the frames riding on top - the switch reading MAC
  addresses and deciding which port each frame leaves by. Cable
  problem means layer 1, switch acting dumb means layer 2. That split
  is why people name the layers when troubleshooting.

## Assessment Questions

1. What is the purpose of the OSI physical layer?  
   Ans: Transmitting bits across the local media.

2. What statement is correct about network protocols?  
   Ans: They define how messages are exchanged between the source and
   the destination.

3. Which three represents standards organization?  
   Ans: IEEE, IANA, IETF

4. What term describes a particular set of rules at one layer that
   govern communication at that layer?  
   Ans: Protocol

5. Which layer of the OSI model defines services to segment and
   reassemble data for individual communications between end devices?  
   Ans: Transport layer

6. What is the purpose of protocols in data communications?  
   Ans: Providing the rules required for a specific type of
   communication to occur.

7. Which term refers to the set of rules that define how a network
   operates?  
   Ans: Standard

8. Which three layers of the OSI model make up the application layer
   of the TCP/IP model?  
   Ans: Application, presentation, and session layer

9. Which organization publishes and manages the Request for Comments
   (RFC) documents?  
   Ans: IETF (Internet Engineering Task Force)

10. Which two OSI model layers have the same functionality as a single
    layer of the TCP/IP model?  
	Ans: Data link and physical layer
