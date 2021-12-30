# -TARP-TEAM-1
## This Project is contributed by 18MIS002 R N Sneha Priya, 18MIS1017 Sandhiya S, 18MIS1090 Raksha S, 18MIS1108 Aishwariya Subakkar, 18MIS1110 Yuktha Sri.c.m. 

There are a series of processes and configuration which are done for the implementation. They are,
- Initially, from the board menu, the board manager is selected from which the ESP8266 is being selected. From the ESP8266 we select NodeMCU 1.0.
- The next setting is to select the COM port. In this the COM 4 is selected from tools and then selecting the communication.
- Then after the code is being developed in the Arduino IDE, it is then compiled to check if there are any error with respect to syntax before it can be loaded into the NodeMCU ESP8266.
- In the newer versions of the NodeMCU the CH34X driver is not included. So, that has to downloaded and has to be installed on the local system on which the Arduino IDE is running.
- Once there are no compilations error found in the code it can now be loaded into the NodeMCU ESP8266 with the help of simple USB cable with Type-A connected to computer and Type-B connected to the NodeMCU board.
- Once the code is successfully embedded in the board, the NodeMCU now has the servomotor controlling code and the web server code which helps in controlling the servomotor with the Wi-Fi module of the NodeMCU ESP8266.
- Now the NodeMCU ESP8266 is now connected to the servomotor with the help of the jumper wires. i.e., the D1 pin of the NodeMCU ESP8266 is connected to the one side of the jumper wire where the other side is connected to the ground of the servomotor.
- Now the servomotor has to be attached with a small slit which basically moves and helps in controlling the food flow into the aquarium. 
- For the ease of both functionality and cost taking into consideration, we have used funnel to hold the fish food. So, the end of the funnel is placed on the top of the slit. So, when the slit tilts according the user input, the food falls down, and when the slit comes back to the original place it will stop. 
- The IP config address of the global IP address to connect and to control the servomotor is 192.168.4.1 in our case. 
- In that IP address there is a small toggle which ranges from 0 to 180 where in 0 is the closed position of the funnel and 180 is the total open position of the funnel which is determined by the slit i.e., when the slit is at 0 then the funnel is closed and when slit is at 180 it is totally opened. 
- So, according to the number of fishes present, the slit can be opened at any angle between 0 to 180 using the toggle in the IP address. This position of the slit can be seen by the serial motor which is basically like the feedback from the sensor present in the motor.
