# Setting Up with Raspberry Pi
## Step 1 Setup the Raspberry Pi
Check out this super quick video on how to setup the Raspberry Pi.
[60 second Raspberry Pi Setup](https://youtu.be/Ewo1NhpivMg)
## Step 2 Connect 
Connect the Zio development board with PM1.0/2.5/10 Sensor to the Raspberry Pi via the ZIO QWIIC HAT.
![PM2.5 Image](https://themachineshop.uk/wp-content/uploads/2019/12/image-15.png)
## Step 3 enable the I2C bus
Either from the Raspberry Pi’s desktop or via SSH, Open the terminal and type in:

`sudo raspi-config` and press enter.
 
Using your keyboards arrow keys, select ‘5 Interfacing Options’ and press enter.
 
Scroll down to `P5 I2C` and press enter.
 
Then select `Yes` and press enter to enable the I2C interface for the ZIO QWIIC ecosystem.
 
Select `Ok` and `Finish` to return to the terminal.
## Step 4 Download python script
Whilst still in the terminal type:

`sudo git clone https://github.com/machineshopuk/PM1.0-2.5-10`
 
This will generate a folder called 2-5PM, enter it by typing:

`cd PM1.0-2.5-10`

## Step 5 Run the script
Then run the script by typing:

`python 2-5PM.py`
 
The script will output PM1, PM2.5 and PM10 values to the terminal in µg/m3. 
