# PPPwnLinux

run commands:
sudo apt install git
sudo apt install python3
sudo apt install python3-pip
pip install scapy
git clone https://github.com/Cyclizar/PPPwnLinux


format flash drive in "disks" as FAT
put goldhen.bin on flashdrive root
put flash drive into ps4
plug in ethernet


run command:
iwconfig

find ethernet ID (should look like "enp0s3...") and copy it
replace <YOURETHERNETID> in ExecuteCMD.txt with your ethernet ID and save the file (ctrl s)
copy all text in ExecuteCMD.txt


in console do:
sudo -i
cd /home/<YOURLINUXUSERNAME>/PPPwnLinux

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
if you get "done" in CMD after about a minute and it pops up saying goldhen on the ps4 you're done, if it fails to find a corrupted object, try it again.
