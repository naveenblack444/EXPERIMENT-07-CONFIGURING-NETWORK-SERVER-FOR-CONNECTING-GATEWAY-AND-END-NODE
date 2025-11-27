### EXPERIMENT -07 CONFIGURING NETWORK SERVER FOR CONNECTING GATEWAY AND END NODE 
 
## Aim: 
To  configure the Network server and end device for transferring data on the network
## Components required: 
End node stm 32 development kit , Dragino LPS8, Network server 

## Theory :
When working with sensitive applications or files, saving progress on your local device is a start, but what if you lose access to your device? Network servers address this problem by hosting the files and programs most pertinent to the network and enabling access for consistent, real-time use. 

As a result, personnel or network clients can instantly access important data or tools while also facilitating collaboration between users. Multiple users can make changes to the same program or document for continued development over the course of a project. Via a secure login, remote users can connect to the home network.
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/59db9b76-ddd5-4d6a-9075-8db233f5e479)


In the above graphic, the circle represents an organization network where a network server facilitates collaboration and file sharing between network clients (devices).

 The role of a network server, then, is to provide users with a set of services and access to resources on the network. These features include:

Permissioned access and log-ins for network users Gateway access to the Internet for an organization Centralized location for network resources  Shared access to devices on the network like a printer or a scanner Hosts multi-user apps like email servers, web applications, or CRM

## Procedure :

 1. login to the network server using login link  https://iot.saveetha.in/
 2. Click on the nework server as shown blow
    
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1bd434ca-1426-4102-8384-94473483543e)
 3. Click on the add gateway 
 
 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/47c2e08d-6598-4437-8b07-f213d6f3b8ac)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/e62ff028-99bc-485e-9808-fbb6e124f8b2)
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/a2e3ae58-6402-49e8-8f96-679059c1842c)
4. Click on the lora options , lora - frequency plan 

5. Click on channels and create a new channel after which you can add a new end device
   
![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/1fb72be5-e48d-4cde-a329-0cfb0d29070f)

6. Add the attributes in the end device as  shown below 

 ![image](https://github.com/vasanthkumarch/EXPERIMENT-07-CONFIGURING-NETWORK-SERVER-FOR-CONNECTING-GATEWAY-AND-END-NODE-/assets/36288975/00bff30b-42fc-42d5-9540-285d270e41cb)
 
7.Using AT commands configure end device in serial port utility
AT Commands to set initially (Mandatory)
 AT+FDR // To do factory data reset
 AT+NJM=1 // To set OTAA mode
 AT+ADR=1 // To enable the ADR
 AT+TDC=600000 // To set the default sampling interval as 10 minutes
(Should not give below 5 minutes)
 AT+CLASS=C // To set class C
 AT+DEUI=XX XX XX XX XX XX XX XX // To set Device EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX // To set APP EUI key
 AT+APPEUI=XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX XX //
To set APP Key
 ATZ // To take effective action on below settings (As like saving)



## OUTPUT 
### BUILD CONFIGURATION
<img width="1920" height="1200" alt="514834955-19ab3d33-bb1a-4f5d-bd11-b376ba2d8224" src="https://github.com/user-attachments/assets/a95610a5-c351-45cd-a86e-571668653e25" />

### AT COMMANDS
<img width="1920" height="1200" alt="514835061-c5d9a1af-7f58-491f-ad4d-c8458733ae0f" src="https://github.com/user-attachments/assets/adf47497-7dff-4863-9793-7585a5c6371b" />
<img width="1033" height="604" alt="514834994-d46e411d-7072-458d-820c-7f427d11c0b5" src="https://github.com/user-attachments/assets/ef91bf09-499b-4f0d-b715-2de55a784f73" />

###<img width="1034" height="597" alt="514835138-596406e1-89eb-42a5-915e-aef98e72b213" src="https://github.com/user-attachments/assets/18754c80-233e-4a81-9b52-031dd4992ebe" />
<img width="1920" height="1200" alt="514835270-d5582420-f8aa-45b6-bcd3-8f6a27bc66c9" src="https://github.com/user-attachments/assets/649fa7d9-660f-42a7-b9b5-61b99e77327c" />
<img width="1920" height="1200" alt="514835314-9716f2c2-34ed-4a4b-b38c-bb6f4a7e3ede" src="https://github.com/user-attachments/assets/65a9c38f-e104-4199-91be-34e6cf4854ef" />
<img width="1920" height="1200" alt="514835476-b6026de6-ca86-4bae-afcb-c16384674b78" src="https://github.com/user-attachments/assets/38ba8971-6acc-48a0-a8a2-0e9c8330b9a1" />
<img width="1920" height="1200" alt="514835514-74ede65f-c989-4500-be2a-8986ea1b0bf4" src="https://github.com/user-attachments/assets/6aadafbe-6844-4bdf-a511-5f1d193b89f1" />
<img width="1920" height="1200" alt="514835544-7dfc3bad-581e-4b47-adb8-50fdbfa8b50b" src="https://github.com/user-attachments/assets/f602ad27-a2b2-40da-82bc-3fce1f8c20e0" />
<img width="1920" height="1200" alt="514835568-080efbd8-268e-4851-8420-208ead1c3d8c" src="https://github.com/user-attachments/assets/22a41b6c-e2e2-4650-9f18-12bd52b04f0f" />

## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
