# 5G-communication-


![Screenshot_2024_1020_230813](https://github.com/user-attachments/assets/1421643d-ec04-4857-affe-828bde1f5449)


![Screenshot_2024_1020_221153](https://github.com/user-attachments/assets/16e30bd4-88ca-43c3-93c6-4ac7cd5cb257)


# ITU (International Telecommunication Union) 
It is a specialized agency of the United Nations responsible for coordinating global telecommunication standards, regulations, and spectrum allocation. It ensures that communication systems worldwide, including telecommunications, radio, and satellite, operate seamlessly and without interference.ITU-R manages radio telecommunication, ITU-T sets technical standards for global telecommunications.


![Screenshot_2024_1020_222847](https://github.com/user-attachments/assets/bb23778f-9dce-4229-991b-71b197e8ae19)

ITU - R -- Radio communication 
ITU -T -- Standardization 
ITU -D -- Development 

# 3GPP 
(3rd Generation Partnership Project) 
•It is a collaborative initiative that develops globally accepted technical specifications for mobile telecommunications. 3GPP defines system architectures, protocols, and standards for mobile networks and works closely with telecom companies and other stakeholders to drive the evolution of cellular networks.

# 5G Use Cases:

1. Enhanced Mobile Broadband (eMBB)

   •provides high speed internet           access and low latency

 2.Massive Machine-Type Communications     (mMTC)
  
   •sports high density of online           devices
   •design to connect large number of       devices and IoT applications.

 3.Ultra-Reliable Low-Latency              Communication (URLLC)
   [key feature of 5G]  
  
   •provides low latency and highly         reliable communication 
   •example- for factory automation,        AR/VR , Remote surgery.etc 

![Screenshot_2024_1020_221601](https://github.com/user-attachments/assets/4107ea1d-4c99-43d7-8e87-02c5a4e74ec1)

## 4G LTE :- 
   a wireless technology that              provides high speed data.
   
  • LTE-- Long Term Evolution 
   (offers fastest mobile internet          experience) 

   
 # 5G Network Components:- 

![Screenshot_2024_1020_223005](https://github.com/user-attachments/assets/82430eec-74b7-4fa2-bedd-541570980642)
 
 ## 1.UE --User Equipment                
   •it means mobile device like           tablet laptop smartphone other         wireless  devices that is used to      access the network
     
## 2.AMF --Access and Mobility Management Function 
   •manage user connections 
   •handles tasks like user               authentication mobility sport          helping devices switch between          different network areas smoothly.

## 3.UPF --User Plane Function 
   •responsible for handling the data       traffic that flows between users        and the internet
   •managers how data is transmitted 
   •acts as a bridge between user          devices and the data services they      access.

## 4.SMF --Session Management Function
   •responsible for setting up,             managing and terminating data           sessions for users.
   •(simply) heads to establish             connections for data services,          controls how data flows.

 ## 5.PCF --Policy Control Function       
   •determines how much data are used      can use privatisation certain          types of traffic and ensures the       network resources are allocated        efficiently.
## 6.UDM --Unified Data Management
   • stores and managers user              information simply it keeps track      of user identities and preferences

## 7.RAN --Radio Access Network   
   •connects user devices to the core      network using radio signals and        enables faster data speed and low       latency.

![Screenshot_2024_1020_221736](https://github.com/user-attachments/assets/1f35296a-e6d4-415e-b739-061a42b2386b)

# Difference between 4G and 5G :-

 •5G have became decentralized forgots   and very flexible. for example 5G      core function can now be co-located    with applications in an edge data      centre, making communication paths     short and thus improving end-to-end     speed and latency.

 •one more concept the distinguishes     5G network architecture from 4G is *edge   computing*

 **edge computing**
 it refers to processing data closer    to  wear it is generated, rather than  sending it all to a central server     for  away. This reduces latency and    improves speed .


# Data Transmission:- 

1. ## Small cells and pico cells:-
   these are low power base stations      used in LTE advanced versions and     5G technology to power devices in      small area like few 100 meters to 2    km

2. ## MIMO:-

![Screenshot_2024_1020_223538](https://github.com/user-attachments/assets/e68eae66-8483-466b-bfc9-6b3aa968e6e2)
   
    Multiple input multiple output

   •involves using multiple antennas at
    both transmeter and receiver .It       allows for receiving and sending       more data at same time, improving      the speed.

![Screenshot_2024_1020_223316](https://github.com/user-attachments/assets/16d6a0e2-3a47-4a64-ae1c-af7a44a3a407)

4. ## Beamforming :-
    •it is a technique that direct          radio signal in specific               direction instead of broadcasting      them in all directions
   *simply*
   it focusee the signal towards a        particular user or device,             improving the quality and strength     of connection.


![Screenshot_2024_1020_223755](https://github.com/user-attachments/assets/d287562c-f04a-49a8-899a-c62a0ff2792d)

5. ## Full Duplex Mode of Transmission:-
    • In this, high speed switches are      used to control data transfer in       each direction by efficiently          switching one at a time and fully      utilising the existing spectrum       .The same frequency band can be         used for transmission and              receiving mode of operation .

# RAN (Radio Access Network) Protocol     Stack:   

## •User Plane Protocol Stack:
   •support carrying the data between       different applications in UE.

## •Control Plane Protocol Stack:
   • carrying control information          between UE and gNodeB or protocol.


# User Plane Protocol Stack:  layers:-

![Screenshot_2024_1020_223845](https://github.com/user-attachments/assets/ef42eafc-efac-4091-a016-cbe852711080)


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

![Screenshot_2024_1020_222043](https://github.com/user-attachments/assets/173ef76f-182a-41b9-abfe-7493b17f5e0e)

## RRC ( Radio resource control)  

  •responsible for setting radio          bearers, system information. 


# Diverse Traffic Types

 There are different types of QoS       flows:-

![Screenshot_2024_1021_071033](https://github.com/user-attachments/assets/0b828114-cd37-4f45-bd89-b09d2eaaa50d)

## Guaranteed Bit Rate(GBR) -->
for critical functions or voice calls. 

## Non-Guaranteed Bit Rate(NGBR) -->  
for streaming or normal broadband connection where steady connection is not required.

*Multiplexing*  occurs at two points in the 5G ran system. The sdap converts IP packets to QoS flows at the core network as per requirement and The upf converts IP flow to QoS flows at the core network. The SDAP maps each flow into radio bearers. The following example helps in understanding this.

![Screenshot_2024_1020_222115](https://github.com/user-attachments/assets/f4fe3571-2f0f-4d68-b8c5-c9948a1d2fe7)


## PDCP
The PDCP does 4 tasks, Firstly it compresses the headers which are 40 bytes in IPv4 and 60 in IPv6 which is almost as large as some smaller data packets, it follows the ROHC(Robust Header Compression).

## Ciphering and Integrity protection: 
Encrypts data and ensures data integrity for secure communication.

![Screenshot_2024_1020_222143](https://github.com/user-attachments/assets/01fffcff-3d46-4ffb-8b04-6b49eb214894)

# MAC(Medium Access Control)
 
  •provide services to RLC in the form   of logical channels and uses           services from PHY layer in the form    of transport channels.

The MAC layer is also responsible for distributing the data into different carriers through multiplexing.

 Since transport blocks can get quite   large we divide it into CBGs (core     block groups), so that if any error    occurs only the CBG needs to be        retransmitted instead of whole         transport block.
 
## Scheduler:-

The function of a scheduler is to allocate when and how much data is to be allocated to different users sharing the same data channel.

![Screenshot_2024_1020_224013](https://github.com/user-attachments/assets/a931265d-8e02-4612-913f-a9bb05b54ebf)

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
   
   
# Modulation Scheme :- OFDM 
 •CAN WE USE TO TRANSMIT A WHITE BAND    SIGNAL USING MULTIPLE NARROW BAND      SIGNALS


***OFDM (Orthogonal Frequency Division Multiplexing)*** is a key modulation technique used in 5G wireless communication. It plays a crucial role in efficiently transmitting data over the air and is also used in earlier standards like LTE.

***How OFDM works:****

***Frequency Division:**** OFDM divides the available spectrum into many narrow frequency subcarriers, typically spaced orthogonally. Each subcarrier carries a portion of the data.


***Orthogonality:*** The orthogonality ensures that there is no interference between the subcarriers, even though they overlap in the frequency domain. This helps to maximize spectrum efficiency.


***Parallel Transmission:**** Multiple data streams are transmitted in parallel across the subcarriers, making it more resistant to interference and signal degradation in environments with multipath propagation (where signals bounce off objects and arrive at different times).
Modulation: Each subcarrier can be modulated using schemes like QPSK, 16-QAM, or 64-QAM (Quadrature Amplitude Modulation), depending on the required data rate and signal quality.


***Why OFDM is important in 5G:**

***High Data Rates:*** OFDM supports high data rates by transmitting multiple bits simultaneously over many subcarriers.

***Resistance to Multipath Fading:***
In urban environments or areas with a lot of signal reflections, OFDM is more resilient than traditional single-carrier modulation techniques.

***Efficient Spectrum Usage:***

The ability to divide the spectrum into smaller subcarriers makes OFDM highly efficient for the dense frequency allocations in 5G.

***Flexible Channelization:***
OFDM allows for flexible channel bandwidths (e.g., 5 MHz, 10 MHz, 100 MHz, or even up to 400 MHz in some 5G configurations), which is critical for 5G's wide range of applications from low-latency services to high-speed data transfer.


**OFDM**is a key technique in 5G because it enables high data rates, reduces interference, and allows efficient use of the radio spectrum in complex environments.


## Disadvantages :- 
it tends to have very high peak power to average power ratio. 

Therefore NR uses -> downlink : OFDM
                     uplink : OFDM 

## OFDM
• each of career carrying complex        symbol for long duration. 
• symbol is spread across a short  
  frequency for long time.

## SC- FDM 
• each of career carrying complex        symbol for small duration. 
• symbol is spread across a wider 
  frequency for shorter time.

# Multiple Access Scheme  :-

- it is a technique that let's multiple mobile users share the allocated spectrum in the most effect of manner.

 # RRC STATES 
   • idle -->used immediately after                 power on.
          -->used for data transfer. 
          -->for all connection 
             related parameters stored              and then device can                    easily go to power saving              mode and then back to     
             connected mode.
             
# Identifiers

Identifiers are used to uniquely recognize any device or subscription to identify its characteristics such as if device is blacklisted or not or any subscription service is allowed or not.

## Types of Identifiers  :-     


## 1. Device Identifiers:

## 1.1 PEI - Permanent Equipment             Identifier

 ![Screenshot_2024_1021_071510](https://github.com/user-attachments/assets/d149a2fc-92e8-4a95-a4ef-5e6bae2c5bd0)

## 2. Subscription Identifiers

## 2.1 SUPI:

MCC : which country subsciber belongs to MNC : defines exact operator in the country MSIN : defines the actual subsciber within operator within the country

![Screenshot_2024_1020_224150](https://github.com/user-attachments/assets/ede1ea6c-f64e-4264-92dc-d8f0002cbdb0)

## 2.2 SUCI: 
 
 Concealed version of SUPI, even if someone "listens" to the signal they will not be able to decrypt it since it is encrypted.

![Screenshot_2024_1020_224226](https://github.com/user-attachments/assets/8ddf6999-7137-434e-8b19-0cf26c8cb870)

#  Service Discovery (NRF)

![Screenshot_2024_1020_224338](https://github.com/user-attachments/assets/4cc8da85-271b-483c-83bb-418d19578868)

## 1. What is NRF?

NRF (Network Repository Function) is a key component in 5G Service-Based Architecture (SBA).

•It enables service discovery, allowing network functions to register and find each other.

## 2. Main Functions:

Registration: Network functions register their services with NRF.
Discovery: NRF provides endpoints of available services to other network functions.


## Load Balancing:

Helps optimize traffic by directing requests to suitable instances.

## 3. RESTful Interface:

Uses HTTP REST APIs for communication between network functions and NRF.

# Registration Management

## 1. What is Registration Management?

It's a process in 5G networks for managing user devices' access to the network.

• Ensures authentication and updates     user information like location.

## 2. Key Functions:

 ##• Registration: Devices (UEs)           register with the network via the      Access and Mobility Management nn      Function (AMF).

 ##• Location Updates: Tracks user          location for efficient resource        allocation.

 ##• Session Management: Enables            network services based on the          user’s subscription and current        location.

# Connection Management

Deals with how a device gets and keeps a connection with the core network.
Sets up, maintains, and ends connections.

## Key Parts:

 ##•Session Setup: Starts                  communication between device and       network.

 ##•Session End: Stops the connection.

 ##•Mobility: Keeps the connection     
    while the device moves.

## RAN Connection Management

•Manages the connection between the device and the Radio Access Network (RAN).

•Makes sure the radio link is stable.

## Mobility Management

•Manages how a device moves around in the network.

•Keeps the connection active as users change locations.

## Session Continuity
 
 •Makes sure that a user's session stays active without interruptions.
Important for maintaining quality during calls or data sessions.

## UDM and UDF

![Screenshot_2024_1021_071818](https://github.com/user-attachments/assets/d451f46d-01dc-47c3-929d-b006da2f1afa)


 # PCF (Policy Control Function)

Central component for managing network policies.

•Controls resource allocation and service quality based on user needs.

# Session Management Policies

•Handles Sessions: Manages the establishment and termination of sessions.

•Quality of Service: Defines how resources are allocated for data and voice sessions.

•Handover Management: Ensures smooth transitions between cells during user movement.

# Non-Session Management Policies

•Network Resource Management: Governs resource allocation without active sessions.

•Access Control: Manages user permissions and service access.

•Traffic Management: Controls data flow and prioritization without maintaining session state.

# Registration

When a device has either moved to a new cell or is connecting to the network for the first time or some other situation, it needs to go through the registration procedure


## For a simple registration the process is as follows:

1.The UE sends the request to nearby RAN which assigns an AMF to the device in one of two ways, either it takes the GUTI(Device Identifier) from the device and assigns it the corresponding AMF it was connected to or it accesses the NSSAI(network slice selection assistance information) to know what AMF supports the network slice and thus foward the request.

2.Context Transfer: Due to device mobility, AMF needs to be switched to a nearby one, in this case new AMF contacts old AMF for UE context transfer.

3.Authentication and Security

4.Context Transfer Completion: New AMF confirms with old AMF that context has been successfully transferred.

5.NewAMF to UDM: New AMF registers with UDM for relevant device and subscription information as well as subscribes to UDM for further subscription updates. Old AMF deregisters with UDM and unsubscribes.

6.Policy Information: New AMF contacts PCF for relevant policy information about the UE.

7.PDU Session Continued/Started: PDU session can be continued or stopped(in case of error) with contact with SMF

8.Registration Complete:Registration completed message is sent by RAN to UE

9.Policy Updation: Any new or updated policies can be fetched from PCF


# Deregistration

When devices no longer needs to access 5G services or network kicks the device out it deregisters.






# 5G course 2 #



# standarization of 5G :-


## ITU-R --International Telecommunication Union Radiocommunication 

•Responsible to develp 5G requirements.

## latency -- 

 the delay between sending and receiving information. 

## mobility --  

Mobility in 5G refers to the ability of a user to remain connected to a network while moving around.

## Usage scenarioes :-

1> Enhanced Mobile Broadband (eMBB) :- Enhanced Mobile Broadband (eMBB) is a 5G service that offers higher data rates, lower latency, and better bandwidth to improve user experience.

2> Massive Machine Type Communication (mMTC) :- Massive Machine-Type Communications (mMTC) is a 5G service category that allows for a large number of devices to connect online. It's designed to support the Internet of Things (IoT) by enabling high-speed, low-latency, and cost-effective communication for many devices with limited data rates.

3> Ultra Reliable And Low Latency Communication :-  it is a set of specifications for 5G mobile networks that enables low latency and high reliability for mission-critical applications.

**5G Architecture** :- 

***Three main components ***

 - UE (User equipment)

 - NG-RAN (Next Generation Radio          Access Network)

 - 5GC (5G Core Network)


## 5G Non Standalone (NSA)
  - Master is eNB . It decides what       type of data is received by the        mobile.

## 5G Standalone (SA)
  -Master is gNB . It decides what        type of data is received by the        mobile.


![Screenshot_2024_1030_101530](https://github.com/user-attachments/assets/c07e1d76-9ca1-401a-8ca0-1c5c9723631e)


-- 4G ran acts as master in NSA, UE       recieves control signalling and        data from master but only data from    secondary

## OFMD :-

-->OFDM works between the UE and the gnodeb.
 
•In OFDM when a signal is at its all time high the other carriers are at 0 because the carriers are placed in such way that they cancel each other out (when overlapped). this is due to some trigo. ofdm is used to transfer many different users' data at once in the same signal and interference is reduced due to this sin cos area(integration) cancellation.
  
--  As frequency of signal increases, there may be interference from other signals, to fix this we have scalable carrier spacing which means the spacing between peaks of any two signals(see below picture) to avoid interference, in LTE this was 15 KHz.
signal peaks




