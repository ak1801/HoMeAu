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
http://winscp.net/eng/docs/scripts,
http://winscp.net/eng/docs/faq_su

#IMPORTANT NOTE:
User osmc is not a root user, it does not have root permissions. To write copy any media in your hard disk, you need to have root level access.
For this you need to add permissions in sudoers file located at (/etc/sudoers).

To can make changes to sudoers from putty/bash:
	Create a back up of this file before editing using -> cp filename{,.bak}
    Type visudo and press enter.
    Navigate to the place you wish to edit using the up and down arrow keys.
    Press insert to go into editing mode.
    Make your changes - for example: user ALL=(ALL) ALL.
    Note - it matters whether you use tabs or spaces when making changes.
    Once your changes are done press esc to exit editing mode.
    Now type :wq to save and press enter.
    You should now be back at bash.
    Now you can press ctrl + D to exit the session if you wish.

