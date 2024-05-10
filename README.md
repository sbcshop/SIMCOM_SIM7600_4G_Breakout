# SIMCom_SIM7600G-H_4G_Breakout

<img src= "https://cdn.shopify.com/s/files/1/1217/2104/files/SIMCOM_4G_module_Breakout_2.png?v=1713787688" />

This Github provides a getting started guide for SIMCom SIM7600G-H 4G Module Breakout.

### Features:
- SIMCom SIM7600G-H 4G Module  
- Status led for board power and Network Activity
- Nano SIM support slot
- Type C interface 
- AT command support for testing functionality and features
- Module functional GPIOs breakout for interfacing
- Interface with various platforms like Arduino, ESP32, Raspberry Pi, etc.
- Multi-constellation GNSS receiver available
- Supported Bands:
    - B1/B2/B3/B4/B5/B7/ B8/B12/B13/B18/B19/ B20/B25/B26/ B28/B66
    - B34/B38/B39/ B40/B41
    - B1/B2/B4/B5/ B6/B8/B19
    - 850/900/1800/ 1900MHz


### Hardware Overview
#### Pinout

<img src= "https://cdn.shopify.com/s/files/1/1217/2104/files/SIMCOM_4G_module_Breakout_Pinouts.png?v=1713787789" />

|									                   |									                |								                |
|------------------------------------|----------------------------------|-------------------------------|
|(1) Auxiliary Antenna SMA connector |(2) Main Antenna SMA connector	  |(3) SIM7600G-H 4G SIMcom Module|
|(4) nano SIM slot  				         |(5) Type C interface              |(6) Module Power BTN    	      |
|(7) NET_STATUS LED                  |(8) Network LED      		          |(9) Power LED                	|
|(10) GPS Antenna uFL connector      |(11) GPIOs and Power Breakout     |	                              |

## Setup to use 4G Module 
- Simply connect breakout to PC/laptop via USB Type C. 

- Now press, hold Power Key button and release after 3-4 seconds to activate module. LEDs associated with the network will light up, first STATUS LED will be on and then NET LED starts blinking. This confirms module ready for use.
  
- To verify open device Manager and check if below listing you can see into COM port. If you cannot see device then driver is missing, download and install driver from [here](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/tree/main/SIMCOM_Windows_USB_Driver)

   <img src="https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/images/device_manager_simcom4g.jpg" width="490" height="400" />
   
- If everything goes well it will connect as a cellular network in your system as shown below. After the succesfull 4G Module connection you will able to use your cellular network to connect with internet.
  
  <img src="https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/images/4g_internet.jpg" width="268" height="411" />

### For AT Commands Testing
- Open XCTU software and select the Serial console option to run as shown below.

  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img1_xctu.jpg" width="490" height="400"/>

- Select Configure option and then suitable AT COM port. Change Baud Rate and other details only if needed, for the 4G module we will keep default settings. Select OK and After that just Close the connection to start.

  <img src="https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/images/configure_comport.jpg" width="490" height="400" />

  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img3_xctu.jpg" width="490" height="400" />

- Now the 4G module is ready to accept AT commands for testing. Either you can send commands through console log or create packets to send AT commands.
  
  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img4_xctu.jpg" width="490" height="400" />

  * AT
  * ATD99########;
  You can refer to the [manual](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/Documents/SIM7500_SIM7600%20Series_AT%20Command%20Manual_V3.00.pdf) for more such AT Commands

- Creating packets is a good option for multiple commands testing. Don’t forget to add 0D and 0A required for carriage return and enter.
  
  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img5_xctu.jpg" width="490" height="400" />
  
  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img6_xctu.jpg" width="490" height="400" />

  <img src="https://github.com/sbcshop/Pico_Cell_4G_Software/blob/main/images/img7_xctu.png" width="490" height="400" />
    
## Resources
  * [Schematic](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout_Hardware/blob/main/Design%20Data/SCH%20Simcom%204G%20bkt.pdf)
  * [Hardware Files](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout_Hardware)
  * [3D Step File](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout_Hardware/blob/main/Mechanical%20Data/STEP%20Simcom%204G%20BREAKOUT.step)
  * [SIMCom SIM7600 4G Module Datasheet](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/Documents/SIM7600%20Series_SPEC_202111.pdf)
  * [SIMCom SIM7600 4G Module Command Manual](https://github.com/sbcshop/SIMCOM_SIM7600_4G_Breakout/blob/main/Documents/SIM7500_SIM7600%20Series_AT%20Command%20Manual_V3.00.pdf)

## Related Products  

  * [Quectel EG25G (4G) Breakout](https://shop.sb-components.co.uk/products/quectel-4g-module-breakout?_pos=2&_sid=5a6b2df96&_ss=r)

    ![Quectel EG25G (4G) Breakout](https://shop.sb-components.co.uk/cdn/shop/files/2quectel.png?v=1713789371&width=150)
    
  * [PiTalk - 4G IoT HAT](https://shop.sb-components.co.uk/products/pitalk-4g-iot-hat-1?_pos=4&_sid=815794148&_ss=r)

    ![PiTalk - 4G IoT HAT](https://shop.sb-components.co.uk/cdn/shop/products/06_2664295e-045b-48c3-bb02-f45ae2d7b4ea.png?v=1677660393&width=150)
    
  * [PiTalk - 2G HAT](https://shop.sb-components.co.uk/products/pitalk-2g-hat?_pos=2&_sid=815794148&_ss=r)

    ![PiTalk - 2G HAT](https://shop.sb-components.co.uk/cdn/shop/products/05_d481ca52-c552-4972-b4b6-d7199af0a3fc.png?v=1674819241&width=150)



       
## Product License

This is ***open source*** product. Kindly check LICENSE.md file for more information.

Please contact support@sb-components.co.uk for technical support.
<p align="center">
  <img width="360" height="100" src="https://cdn.shopify.com/s/files/1/1217/2104/files/Logo_sb_component_3.png?v=1666086771&width=300">
</p>

