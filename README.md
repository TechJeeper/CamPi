# CamPi WiFi Camera Controller

CamPi is a WiFi camera controller that uses a Raspberry Pi.  

![alt text](https://github.com/TechJeeper/CamPi/blob/06448bcaf05bdaf52368d965974d110b10606ec7/Screenshot_20211114-144331.png)

## Hardware
CamPi can be ran on pretty minimal hardware.  For my project I am using a Pi Zero W 2 with a SugarPi power hat. 

USB OTG cable that fits your camera and the USB port on the Pi

![alt text](https://github.com/TechJeeper/CamPi/blob/06448bcaf05bdaf52368d965974d110b10606ec7/PXL_20211116_203207215.jpg)

## Installation

From Image:

Flash the latest CamPi img file to the SD card used for your Raspberry Pi - the image can be downloaded at https://techjeeper.com/CamPi_v1.img.zip

From Scratch: 

If you'd like to build it from scratch on your own, here are the components I used. 

I started with a base Raspbian build.
Installed a captive WiFi portal using this guide,
https://www.ralfweinbrecher.de/post/automatic-wifi-hotspot-on-raspberry-pi-zero-w-to-setup-wifi/

I then installed Node-Red with Node-Red Dashboard using this guide, 
https://nodered.org/docs/getting-started/raspberrypi
 
I installed gPhoto2 to control the camera following this guide,
https://pimylifeup.com/raspberry-pi-dslr-camera-control/

Finally I created a custom Node-RED stream and Dashboard to control the camera that I will share to the Github Repo. 

## Usage

When you power on the Pi, after a few seconds you should see a new Wireless Network.  Connect to that wireless network with your mobile device and it should open the camera controller.  If not, navigate to http://10.0.0.1 from your browser while connected to the CamPi wireless network. 

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
