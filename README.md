# Lora-Network

I created a basic Lora network using
- #### Arduino as a micro controller
- #### [Lora Dragino shield  link](https://www.dragino.com/products/lora/item/102-lora-shield.html)
- #### Raspberry pi 
- #### [Raspberry pi Lora hat  link](https://www.antratek.com/raspberry-pi-lora-gps-hat-868mhz)

- #### As a back-end server i used Node-Red 
- #### To control the system , i used an iOS application as interface  


# Architecture of the network 

![alt text](https://github.com/hilalalhakani/Lora-Network/blob/main/Screen%20Shot%202021-08-16%20at%205.35.00%20PM.png?raw=true)

The arduino communicate with each others using Lora technology , the data is saved using SQLite on the pi 
the communication between the ios application and pi is done using API request via Node red 

the code of the arduinos is found at https://github.com/dragino/Lora
the code of the piHat is found at https://codeload.github.com/dragino/rpi-lora-tranceiver/zip/master

# Setup Raspberry pi Hat 
after Downloading the pihat code 
change directory to rpi-lora-tranceiver/ dragino-lora-app-w1 
then enter the following commands

![alt text](https://github.com/hilalalhakani/Lora-Network/blob/main/Screen%20Shot%202021-08-16%20at%205.50.34%20PM.png?raw=true)

if no text was entered , the pi is in receiving mode 

![alt text](https://github.com/hilalalhakani/Lora-Network/blob/main/Screen%20Shot%202021-08-16%20at%205.55.34%20PM.png?raw=true)

 Make sure that the pi and the arduinos have the same frequency and SF 

