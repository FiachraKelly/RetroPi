# RetroPi
This is the write up for the retro entertainment system that I have been working on

For the basic start up (the hardware)
  You will have two boards for this project, the Pi board and the Arduino board, both of these are linked together via a USB cable.
  The first board is your primary board is the Raspberry Pi board; this is what is going to be the core of everything, on the Raspberry pi
  Board there are four USB ports, one Micro USB port and a HDMI port, this port you will need to plug in a HDMI to VGA converter, on
  This converter there will be an audio jack, this is where you will put the speakers that you have, and you must make sure that the cable
  Is secure from the HDMI port to the Screens port. You only need one port from the four USBs; you will need to power the other board
  And to do this you will need a micro USB to go into the Arduino board. This board will be in charge of the controls.
  
  The Arduino board 
    This board is responsible for your controls, how they work and where they are mapped to.
    The board itself as a power supply which is where the micro USB will go to give it power and this will be connected to the pi itself
    It also has two sets of pins running either side of the board, the pins that run along the same side as the power input will be the control pins which are what you will use to map out the controls that you have made (see the map below)
    The other side of the board opposite the control pins are the ground pins this is what will give the buttons and joystick power.
    These will be inserted into the part of the board that says the voltage, depending on wat one you have is the one that you select
    
  The buttons
    The buttons are the easiest to set up; you need to link all the buttons with the ground wire.
    To do this you find the ground pin (middle pin) then add the wire to it through a tag, after you do this you need to link that button up to the other button by doing the same process.
    After you get the buttons linked together, you now need to go and link them to the joypad, to do this, it is the same process, the joysticks ground pin will be the ones that are sticking out when you go and look at it. When you get these done you will now have power to these components.
    
  Setting up the buttons
    once you get power to the you then need to give them their controls, to do this you need to find the command pin which is the bottom pin for the buttons and the pins that are left on the joystick, this set up is the same as the buttons. Once you have that done instead of putting the wire into the slots where the power cable is you will put it into the opposite side, this will link the buttons to the button map.
    
    Button map
      0 = up
      1 = down
      2 = left
      3 = right
      4 = A
      5 = B
      6 = X
      7 = Y
      8 = Start
      9 = Select 
      
      *note*
      You can change the controls at any time 
      
      When downloading roms use the rom set .78 they seem to be the only ones that work currently
      
      If you want to use the speakers withot having a wire going from the speakersto an outlet which would be outside the biuld of the table I would get a stronger power supply, currently I am using a 2.5 amp to power the Pi, if you want to use the Pi to power te speakers, you should bet a 3 or 3.5 amp fuse, this way you can use the speakers in the table without the need of an extrnal power supply for just the speakers  
      
      
      *links*
        *roms*
         https://archive.org/details/MAME0.78-MAME2003-ROMs-CHDs-Samples
         http://www.emuparadise.me/roms/search.php?query=.78+rom+set&section=all
            
            *how to set up the second board*
            https://www.element14.com/community/servlet/JiveServlet/downloadImage/102-80946-11-252309/837-439/Leonardo+Controller+Wiring.png
            

