# PPPwnLinux

# YouTube Guide:
https://www.youtube.com/watch?v=7-7Tot0-868



# about
this is just SiSTRo's PPPwn (https://github.com/sistr0/pppwn) with his goldhen and stage2 all in one place, and the instructions are designed around linux. was able to get this running on my lenovo t470 dualbooting linux mint 21.3, and my macbook pro 2012 primarily running linux mint cinnamon 21.2. windows sucks for this exploit, so use linux!! trust me its better. 



# run commands
sudo apt update && sudo apt upgrade
sudo apt install git
sudo apt install python3
sudo apt install python3-pip
pip install scapy
git clone https://github.com/Cyclizar/PPPwnLinux



# flash drive setup
format flash drive in the linux app "disks" as FAT
put goldhen.bin on flashdrive root
put flash drive into ps4
plug in ethernet



# setting up the command to execute the script
run the command:
iwconfig

find ethernet ID (should look like "enp0...") and copy it
replace <YOURETHERNETID> in ExecuteCMD.txt with your ethernet ID and save the file (ctrl s)
copy all text in ExecuteCMD.txt



# executing the exploit
in console do:
sudo -i
cd /home/<YOURLINUXUSERNAME>/PPPwnLinux
^^ (or cd wherever the PPPwnLinux folder is located)
paste command copied from ExecuteCMD.txt with right click > paste, don't execute yet

on ps4 go to: 
Settings > Network > Set Up Internet Connection

set the settings as follows:

Use a LAN Cable
Custom
IP Address Settings: PPPoE
Username: anything
Password: anything
DNS Settings: Automatic
MTU Settings: Automatic
Proxy Server: Automatic


hover over "Test Internet Connection" on PS4 and the enter key on the pc/laptop (while in cmd with sudo -i active and the command from ExecuteCMD.txt in the text field)
press both at the same time and wait
if you get "done" in CMD after about a minute and a notification pops up saying goldhen on the ps4 you're done, if it fails to find a corrupted object, try it again.

# if there are any issues with this add me on discord @3ar and ask.
