## 5G RAN

This can operate in two frequency ranges 

• FR 1 -- 450-6000 KHz

• FR 2 --24250-52600 MHz

• below 1GHz --> excellent for large areas,
             --> excellent in building pentration.
             
OFMD :-

-->OFDM works between the UE and the gnodeb.

• In OFDM when a signal is at its all time high the other carriers are at 0 because the carriers are placed in such way that they cancel each other out (when overlapped). this is due to some trigo. ofdm is used to transfer many different users' data at once in the same signal and interference is reduced due to this sin cos area(integration) cancellation.

-- As frequency of signal increases, there may be interference from other signals, to fix this we have scalable carrier spacing which means the spacing between peaks of any two signals(see below picture) to avoid interference, in LTE this was 15 KHz. signal peaks            

***(AS CAREER SPACING INCREASES -- TIME SLOT OCCUPIED DECREASES)***

## FRAME STRUCTURE:- 

1slot = 14 OFDMA 

![flexibleslotdivision](https://github.com/user-attachments/assets/f46c7275-f851-4b97-a695-8b8f549bdb5b)


12 Subcarriers = 1 Resource Block 


![frames](https://github.com/user-attachments/assets/9bcdc580-306a-4eea-85f1-f2f9f454ef07)

***more resource block given to a cell --- more is the data rate.*** 

• in LTE , resource block is defined in both time and frequency domain. 
• in 5G , resource block is defined in frequency domain only. 

=> in favourable conditions:- 
     5G use 256 QAM ( Qaudrature Amplitude) because it provides 8 bits per symbol transmission        rate.
=> and 64 and 16 QAM in did you deteriorat condition  as it probides 6 bits and 4 bits / symbol.


![resoruceblcok](https://github.com/user-attachments/assets/51f2c910-2d4c-405e-8ae7-4d93f04b2f2b)

![resourceelement](https://github.com/user-attachments/assets/0758cd3f-584c-422b-8cd3-9ae7b8bcdd52)


## Cloud RAN :-
 [ BASICALLY MODIFY ARCHITECTURE OF NEXT GENERATION .]

 • easy scaling up. 
 • on demand resource allocation. 
 • reduced cost.

 ***1. Distributed Unit ( DU)***
     only transmit and receive signals. 

***2. Centralised unit (CU )***
    handle scheduling--- like what resources in terms of resource block are allotted to the                               mobile phone
    handle security --- like the user data is encrypted, user authentication. 











    
    
