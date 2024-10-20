# 5G-communication-

# ITU (International Telecommunication Union) 
It is a specialized agency of the United Nations responsible for coordinating global telecommunication standards, regulations, and spectrum allocation. It ensures that communication systems worldwide, including telecommunications, radio, and satellite, operate seamlessly and without interference.ITU-R manages radio telecommunication, ITU-T sets technical standards for global telecommunications.

ITU - R -- Radio communication 
ITU -T -- Standardization 
ITU -D -- Development 

# 3GPP 
(3rd Generation Partnership Project) 
•It is a collaborative initiative that develops globally accepted technical specifications for mobile telecommunications. 3GPP defines system architectures, protocols, and standards for mobile networks and works closely with telecom companies and other stakeholders to drive the evolution of cellular networks.

# 5G Use Cases:

1. Enhanced Mobile Broadband (eMBB)

   •provides high speed internet access     and low latency

 2.Massive Machine-Type Communications     (mMTC)
  
   •sports high density of online           devices
   •design to connect large number of       devices and IoT applications.

 3.Ultra-Reliable Low-Latency              Communication (URLLC)
   [key feature of 5G]  
  
   •provides low latency and highly         reliable communication 
   •example- for factory automation,        AR/VR , Remote surgery.etc 

## 4G LTE :- 
   a wireless technology that              provides high speed data.
   
  • LTE-- Long Term Evolution 
   (offers fastest mobile internet          experience) 

   
 # 5G Network Components:- 
 
 ## 1.UE --User Equipment                  •it means mobile device like tablet     laptop smartphone other wireless        devices that is used to access the      network
     
## 2.AMF --Access and Mobility Management Function 
   •manage user connections 
   •handles tasks like user                authentication mobility sport           helping devices switch between          different network areas smoothly.

## 3.UPF --User Plane Function 
   •responsible for handling the data       traffic that flows between users        and the internet
   •managers how data is transmitted 
   •acts as a bridge between user           devices and the data services they      access.

## 4.SMF --Session Management Function
   •responsible for setting up,             managing and terminating data           sessions for users.
   •(simply) heads to establish             connections for data services,          controls how data flows.

 ## 5.PCF --Policy Control Function       
   •determines how much data are used      can use privatisation certain          types of traffic and ensures the       network resources are allocated        efficiently.
## 6.UDM --Unified Data Management
   • stores and managers user              information simply it keeps track      of user identities and preferences

## 7.RAN --Radio Access Network   
   •connects user devices to the core      network using radio signals and        enables faster data speed and low       latency.

# Difference between 4G and 5G :-

 •5G have became decentralized forgots   and very flexible. for example 5G      core function can now be co-located    with applications in an edge data      centre, making communication paths     short and thus improving end-to-end     speed and latency.

 •one more concept the distinguishes     5G network architecture from 4G is *edge   computing*

 **edge computing**
 it refers to processing data closer    to  wear it is generated, rather than  sending it all to a central server     for  away. This reduces latency and    improves speed .


# Data Transmission:- 

1. ## Small cells and pico cells:-
   these are low power base stations      used in LTE advanced versions and     5G technology to power devices in      small area like few 100 meters to 2    km

2. ## MIMO:-
   Multiple input multiple output

   •involves using multiple antennas at
    both transmeter and receiver .It       allows for receiving and sending       more data at same time, improving      the speed.

4. ## Beamforming :-
    •it is a technique that direct          radio signal in specific               direction instead of broadcasting      them in all directions
   *simply*
   it focusee the signal towards a        particular user or device,             improving the quality and strength     of connection.

5. ## Full Duplex Mode of Transmission:-
    • In this, high speed switches are      used to control data transfer in       each direction by efficiently          switching one at a time and fully      utilising the existing spectrum       .The same frequency band can be         used for transmission and              receiving mode of operation .

# RAN (Radio Access Network) Protocol     Stack:   

## •User Plane Protocol Stack:
   •support carrying the data between       different applications in UE.

## •Control Plane Protocol Stack:
   • carrying control information          between UE and gNodeB or protocol.


# User Plane Protocol Stack:  layers:-

## 1.PHY (Physical Layer):

•Responsible for efficient wireless     communication.

(there is a need of feedback to know if transmission is error free or not , so MAC comes in role )

## 2.MAC (Medium Access Control):

 •used in re-transmission,              multiplexing, de-multiplexing.

 (not all errors can be detected by MAC. so RLC is used )

## 3.RLT (Radio link Control):
 •implements ARQ for error correction. 
 •handles segmentation, breaking up      data packets into smaller segments.

## 4.PDCP (Packet data convergence         protocol)
  •IP header stores information that      is not necessary so headed is          compressed, remove duplicates,         integrate protection. 

## 5.SDAP (Service Data Adaptation Protocol):

 •Matches the appropriate QoS bearer     to the correct radio bearer.
  For example, a voice call packet is    treated differently from a streaming   packet.  

# Packet Flow Through 5G Protocol Layers:- sdu/pdu

## SDU and PDU:

SDU (Service Data Unit): Data received from the layer above.
PDU (Protocol Data Unit): Processed data with added headers, passed to the next layer.


# Control Plane Layer :-

## NAS ( Non access stratum)
  
  •it includes authentication,           security, idle mode procedures.
  •also responsible for assigning an     IP address to the device.

## RRC ( Radio resource control)  

  •responsible for setting radio          bearers, system information. 


# Diverse Traffic Types

 There are different types of QoS       flows:-

## Guaranteed Bit Rate(GBR) -->
for critical functions or voice calls. 

## Non-Guaranteed Bit Rate(NGBR) -->  
for streaming or normal broadband connection where steady connection is not required.

*Multiplexing*  occurs at two points in the 5G ran system. The sdap converts IP packets to QoS flows at the core network as per requirement and The upf converts IP flow to QoS flows at the core network. The SDAP maps each flow into radio bearers. The following example helps in understanding this.

 ## PDCP
The PDCP does 4 tasks, Firstly it compresses the headers which are 40 bytes in IPv4 and 60 in IPv6 which is almost as large as some smaller data packets, it follows the ROHC(Robust Header Compression).

## Ciphering and Integrity protection: 
Encrypts data and ensures data integrity for secure communication.

# MAC(Medium Access Control)
 
  •provide services to RLC in the form   of logical channels and uses           services from PHY layer in the form    of transport channels.

The MAC layer is also responsible for distributing the data into different carriers through multiplexing.

 Since transport blocks can get quite   large we divide it into CBGs (core     block groups), so that if any error    occurs only the CBG needs to be        retransmitted instead of whole         transport block.
 
## Scheduler:-

The function of a scheduler is to allocate when and how much data is to be allocated to different users sharing the same data channel.

## Downlink Scheduling

The scheduler also decides what amount of bandwidth is to be used by the device as per the service it is providing. This is known as *reciever-bandwidth adaptation.*

*Preemption*:- refers to the ability of the network to interrupt or replace lower priority task or users to allocate resources for higher priority tasks.

# Physical Layer:- 
  •mainly mapping transport channels     to the physical channels

## 1. PBCH (physical broadcast              channel)
   •carries path of the system             information that to access the         network 

 ## 2. PDSCH (Physical Downlink Shared       Channel)  
   •for data transmission to the           devices 

## 3. PDCCH (Physical Downlink Control       Channel)   
   •control information like               scheduling decisions 

## 4. PUSCH (Physical Uplink Shared          Channel)  
   •main channel for data transfer 

## 5. PDCCH (Physical Uplink Control         Channel)      
   •for scheduling decisions
   
   


