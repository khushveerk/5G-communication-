# gNB :- 
## function :- 

• transmission and reception of radio signal as it is responsible for communicating with UE 

• manage radio resources like what we shows in terms of resource block are located to mobile phone.

## Access Stratum Signalling 

-- which is going on between UE's and gNB . 

## Non-Access Stratum Signalling 
-- which is going on between UE and core network 


**PDU sessions and QoS Flows**

5G is an **All IP Service**  all data is transferred through packets.
A pdu(protocol data unit) session is started to connect UE to the internet.
Different QoS flows are determined in that PDU according to the data type 
flowing through it.

![pdu+qos](https://github.com/user-attachments/assets/5b84b55d-c1fc-4d67-baa0-ef2264550bf5)


## the whole ___ is divided into two planes .
1. user plane
2. control plane

 this is called **Control Plane Separation**

• Data flows only through the user plane.  

![userplanecontrolplaneseparation](https://github.com/user-attachments/assets/d35a3470-1507-4340-99ad-17e2c5a319d1)

The advantage of separating these planes is that we can easily scale up or down according to user and control plane requirements. Thus saving resources and money.
