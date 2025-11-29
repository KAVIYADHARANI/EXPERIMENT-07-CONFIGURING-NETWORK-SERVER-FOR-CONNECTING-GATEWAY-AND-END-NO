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


<img width="1920" height="1200" alt="Screenshot (55)" src="https://github.com/user-attachments/assets/d179f47f-f0cc-476d-b632-cef0890146a9" />

![1567ba25-0b85-4ce3-9918-4cf746d74a1c](https://github.com/user-attachments/assets/9ec97522-840a-4f77-9654-a0343c5ed775)

![09b44da8-054f-4b2c-bc90-037f5eba77c2](https://github.com/user-attachments/assets/8def4d8f-4900-4d8a-89b8-0b887a02fa68)

![1fac94da-06fc-40e3-be92-dd6f421a089e](https://github.com/user-attachments/assets/ddb78698-92c1-4614-b13f-dfa445db2a99)


![ad507ee5-a573-4990-9bf9-21695b440c44](https://github.com/user-attachments/assets/4f4ce06d-905a-40b1-95c5-b53f1736818f)

![0adf6648-7045-46ed-b524-7da96de9e36a](https://github.com/user-attachments/assets/4b25f90e-e3d0-4de4-829b-1f611a22b33f)


![16054210-06fe-4030-bac8-26c398192d6f](https://github.com/user-attachments/assets/71b81bed-8e58-4e47-a031-2385f66df886)


![3a8939db-63c3-4fda-9fe8-022ef8f58d35](https://github.com/user-attachments/assets/d12e4228-fae7-476f-b679-4fc21cd46b38)


![f6843d76-867e-46c3-8281-23ba3bb7431a](https://github.com/user-attachments/assets/2a1d1884-468b-482c-887e-82ff5aa482d3)


![d87e63c4-5fb8-422e-8ec6-49cb3f7d5f83](https://github.com/user-attachments/assets/15661809-c960-4c72-8bf8-05ce1e4056b4)


![ee3572ad-7061-42ee-837d-0638cf1cf134](https://github.com/user-attachments/assets/78ca8f37-5cd5-4bd1-be73-3c7afdf97042)



![ce03696d-d9ba-43a4-8a46-3694d0f5ee8d](https://github.com/user-attachments/assets/8736fa32-1874-40bf-a3ea-b2068053b706)


![894fafe9-fb74-450f-b6b0-68b23daf2f13](https://github.com/user-attachments/assets/e18c3da8-f478-49bc-9d48-3eff9b49a27b)







## Result: 

  The Network server and end device for transferring data on the network has been accomplished.
