# **IoT smart weather project:**

## Aim:  
- To understand STM32F01RBT6 ARM cortex M4 Microcontroller and serial communication protocols (UART and I2C) 

## Hardware information:
<ul>
       <li> STM32F01RBT6 - Microcontroller</li>
       <li> LM3502  - Temperature Sensor</li>
       <li> DS1307  - Real Time Clock</li>
       <li> AT24C08 - eeprom</li>
       <li> ESP8266 - WiFi</li>
       <li> 16X2 LCD Display</li>
</ul>

## Software information:
<ul>
       <li> keil uvision 5</li>
       <li> STLINK V2 Debbuger</li>
</ul>

## Basic Working:
<p>  
       <ul> - Initialization part<br>  
        - infinite Loop:<br>  
              <ul>        <li>     ADC_converstion (every 1 sec) <br>  </li>
                         <li>  Get data from RTC and print in display (every 1 sec)<br>  </li>
                         <li>  Send data to cloud (every 4-5 sec)<br>   </li>
                         <li>  Store and read from EEPROM (every 1 sec)<br> </li>
        </ul></ul>
        <ul>- Switch<br>                    
                      <ul><li> SW1 pressed: write the RTC date<br>  </li>
                          <li> SW2 pressed: EEPROM data displayed   </li>
        </ul></ul>
  </p>  

## This Project done in 3-different versions
 <ul>  
       <li> IoT smart weather project V1 (Without i2c)</li>
       <ul>
           <li> Read data from LM35 sensor and display in 16x2 LCD display, Simultaneously sends data to the cloud</li>
       </ul>
       <li> IoT smart weather project V2 (With WiFi)</li>
       <ul><li> Read data from LM35 sensor and RTC display content in 16x2 LCD display, Simultaneously sends data to the cloud and store values in EEPROM</li></ul>
       <li> IoT smart weather project V3 (With Wifi and if WiFi connection disconnected then data stored in EEPROM)</li>
       <ul><li> Read data from LM35 sensor and RTC display content in 16x2 LCD display, Simultaneously sends data to the cloud </li>
       <li> In case the data transmit fails then turned ON RED LED and then store data in EEPROM</li>
       <li> Display "ERROR" message in 16x2 LCD</li></ul>
 </ul>
