# HoMeAu
HoMeAu is an IoT project on Home Media Automation using OSMC and Rasberrypi.

Are you fond of watching movies on your big LED/LCD TV? Yes? But you do not have a media device that can directly run your movies as soon as they are downloaded in your computer!

HoMeAu is the solution for you. It is very simple, inexpensive & easy to configure solution which can be setup in a few hours.
Just follow the steps below and stay excited to create your own media automation!

Step1 - Setting up OSMC on Raspberry Pi.
->Download OSMC from this link https://osmc.tv/download/
->Install OSMC on the SD card, setup wireless connection by connecting Raspberry Pi with your home network (Wifi hotspot) at the time of installation.
->Insert the SD card in the Pi, connect the Pi with ethernet cable or wifi dongle, keyboard, mouse and HDMI cable before powering it on.

Step2 - Configuring unique ip address for listening on OSMC.

Step4 - Installing Kore Android/IOS application in your smart phone to control the media on OSMC.

Step5 - Connecting hard disk with OSMC installed Raspberrypi.

Step6 - Configure Kore app to listen on configured IP address.

Step7 - Run winscp script - media_push.txt to push any media file to desired location on the hard disk.
Execute following command in cmd from winscp installation directory:
winscp.com /script=media_push.txt

Step8 - Automate the script for scheduled file transfer & sync local media directory with remote media directory.

Resources:
http://winscp.net/eng/docs/scripts
http://winscp.net/eng/docs/faq_su
