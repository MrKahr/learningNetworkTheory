# Review Questions 

## R1
In the terminology of CNTDP, there is no semantic difference between a host and an end system, they both refer to termnial nodes in a network.  

Some end systems include: 
- A phone 
- A table 
- A home computer 
- A smart Fridge 
- A sat-navn 
- A Web-server 
- A Mail-server 
- A Game console 

## R2
One possible greeting protocol: 
- Greeting 
- Greeting 
- Pleasantries
- Pleasantries  
- Information 
- Question 
- Reply 
- Farewell 
- Farewell


## R3
Internet protocols is a set of rules that systems follow to transfer data between each other in a network.  
Standards are important because they allow systems in a network to synchronize the transfer of data, avoid wasted i.e. if one system experiences congestion, accurately transfer information across many systems.

## R4
- Ethernet - Home/enterprise 
- Wifi - Home/enterprise 
- Coaxial cable (e.g. in broadband) - Home
- DSL (digital subscriber line) - Home 
- 5G (public) - wide area access 

## R5
In Hybrid fiber-coaxial HFC, optical fiber carries signals from an ISP's headend to a fiber node.  
The fiber node converts the signal from an optical signal to an electrical signal which is distributed over coaxial cables that connect the fiber node to end systems (usually homes) that share bandwidth. All downstream packets orignate from a single head and there are therefore no collisions. (p 44-45)

## R6
Access technologies that are considered inexpensive to install, maintain and that do not have to server many users at a time. 

These could include: 
- DSL - possible through already connected phone cables 
- 5G - great range that can serve a good number of users

## R7
DSL is considered faster than dial-up because of DSLs make use of signmal segmentation. DSL uses a splitter and a formatter (DSLAM) to create three different frequency bands to send and recieve data: a high-speeed downstream channel (50kHz-1MHz), a medium speed upstream channel(4kHz-50kHz), and a two-way telephone channel(0-4kHz). Due to the higher frequency bands, DSL can transfer data much faster than a dial-up connection that has to use the slow telephone channel.   


## R8
Some possible physical media that can be used to run an ethernet over
- twisted-pair copper wires 
- coaxial cable 
- fiber optic cables

## R9
{download/upload}
- HFC: {40Mbps/1.2Gbps}, bandwidth is shared 
- DSL: {24-52 Mbps/3.5 Mbps}, bandwidth is not shared 
- FTTH: {Gpbs?}, bandwidth is not shared 

## R10
Different wireless technologies that I often use: 
- Bluetooth - transmits data between systems using radio waves. It has a relatively short range (10m) and permits a limited number of end systems as part of the network at any given time. Mainly used for inter-device communication. Creates its own network rather than relying on a router. Less secure since no password is required. Due to signal strength, more prone to intereference. 
- Wifi - similarly transmits data between systems using radio waves. Has a longer range (50m). Mostly used for smaller network communication. Connects devices via a router. Often requires a password to access. 
\
As a user, I care about the speed at which data is initially sent to my device (total delay) and data transfer speed that I can expect (average throughput), and the range that is required to connect to the network.  

## R11
Using the assumptions provided in R11, assume that one packet P of length L bits is being sent between switching and recieving host. 

To successfully transmit the packet, all bits of P must reach both the switch and the host machine.

At time $t_0$, the sending host begins transferring the packet to the switch that finishes recieving the packet at time $L \cdot  R_1$ assuming no propagation delay. From the the switch begins sending the packet at time $L \cdot R_1$. By assumption, the switch transfers the packet in time $L \cdot R_2$. 

The end to end delay E, can therefore be modelled as a sum of transfers required for the packet to reach the recieving host: \
$E = L (R_1 + R_2)$

## R12
Advantages of
Curcuit vs packet switching
- Maximal use of bandwidth to transmit messages since there are no competing connections/packets. 
- Delays such as the processing delay are not present in circuit switching. 
- Dedicated conneciton eliminates data loss due to network congestion. 

TDM over FDM in a circuit switched network
- FDM requires hardware to shift/transform signal into different frequency bands. This is not the case with TDM, which does require a queue algorithm to allocate timeslots to packets. 


## R13
- A: Supposed each users transmits continously at 1 Mbps. Circuit switching shares bandwidth equally between users. Therefore, a total of 2 users can be supported at any one time, since each user requires 1 Mpbs throughput of the link. 
- B:Suppose packet swithcing is used. Each user frequires 1 Mbps to send their packet. It is possible for two users to send their data with neligible queing delay because a the required maximal capaciity of 2 Mbps of bandwidth is available. The bandwidth required for 3 users to send data is 3 Mpbs which is why at least one user will experience processing delay.   
- C: This is given in the problem as 20%. 
- D: We assume that users transmitting data are independent events. We assume that the probablity of three users transmitting data can sampled from a binomal probablity distrbition. We use this distrbition to find the proability of three users simultanously transmitting data as:  

$P(X = 3) = \binom{3}{3}0.2^3(1-0.2)^{3-3} = 0.2^3 = 0.008 $ 


## R14
(ISP): Internet service point.

(IXP): Internet exchange point. 

It is sometimes beneficial for ISPs to send traffic to each other e.g. to improve transfer speed of data (see the trombine effect https://www.cloudflare.com/learning/cdn/glossary/internet-exchange-point-ixp/)

If ISPs do not peer, they will have to send traffic through an intermediary ISP which they will have to pay for processing the traffic.  

When two ISPs peer, they can reduce their payments to provider ISPs.  

An IXP is a node that allows ISPs to meet. 
IXP's earn money by charging a few for each ISP that establishes a connection. This fee may depend on the traffic that is sent from a given ISP. 

## R15


## R16

## R17

## R18

## R19 

## R20

## R21

## R22

## R23

## R24

## R25

## R26

## R27

## R28