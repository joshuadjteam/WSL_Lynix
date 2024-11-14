Hello guys!

Here at DJTeam we've been working on Lynix to Linux (Work in progress with WSL) and its a sucess!
To Buy the New version (1.2.1a) goto https://lynixity.x10.bz/

For a Video... goto 

REQUIRED ITEMS
- Intel Vt-x or AMD V
- Windows 10 or higher
- 5 GB RAM
- 50 GB free of space Recommened or 25 GB Minimum (This is used for every user)

SETUP WSL

1. Set up your WSL enviorment (preferred Ubuntu)
2. open your start menu and type "Turn Windows Features On or Off"
3. open the app and choose "Windows Subsystem for Linux (WSL)" and "Hyper-V"
4. Then it'll prompt you to restart your PC - do that
5. After a log in open Powershell as an Administrator

INSTALLING WSL

run the first Command
wsl --install

Now wait and sit back (this may take a few minutes to 5 hours - IM NOT JOKING lol)
And setup your UNIX account
sudo -i

Enter these commands

echo This requires an Admin account... use sudo -i to load the superuser

echo THIS REQUIRES A SUPERUSER ACCOUNT!!!!

sudo apt update && apt upgrade

sudo snap install discord

sudo snap install brave

sudo apt install cinnamon -y

sudo snap install firefox

sudo apt install x11-apps -y

sudo apt install ubuntu-desktop

sudo apt install xfce4 xfce4-goodies && echo On xfce4 choose gdm3 when prompted

sudo apt install xrdp -y

sudo echo "xfce4-session" | tee .xsession

systemctl restart xrdp

sudo apt install gedit -y

sudo apt install gimp -y

sudo apt install nautilus -y

wget -O - https://dl.winehq.org/wine-builds/winehq.key | sudo apt-key add -

sudo add-apt-repository 'deb https://dl.winehq.org/wine-builds/ubuntu/ jammy main'

sudo apt install --install-recommends winehq-stable

sudo apt upgrade winehq-stable

sudo dpkg --add-architecture i386

sudo apt install wine64 -y

sudo apt install wine32:i386

sudo apt install libwine -y

sudo apt install vlc -y

sudo apt install yum

sudo apt install dnf

cd /tmp

sudo wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

sudo dpkg -i google-chrome-stable_current_amd64.deb

sudo apt install --fix-broken -y

sudo dpkg -i google-chrome-stable_current_amd64.deb

sudo apt-get install -y nautilus gedit

sudo apt-get install wget ca-certificates

sudo snap install --classic code

sudo add-apt-repository "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main"

sudo apt update

sudo apt install code && echo this is Visual Studio Code

sudo snap install code

passwd root

wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | gpg --dearmor | sudo tee /etc/apt/trusted.gpg.d/sublimehq-archive.gpg > /dev/null

echo "deb https://download.sublimetext.com/ apt/stable/" | sudo tee /etc/apt/sources.list.d/sublime-text.list

sudo apt-get install apt-transport-https

sudo apt-get install sublime-text

sudo apt install curl ca-certificates -y

curl -s https://repo.waydro.id | sudo bash

sudo apt install waydroid -y

sudo apt-get install libc6:i386 libncurses5:i386 libstdc++6:i386 lib32z1 libbz2-1.0:i386

sudo yum install zlib.i686 ncurses-libs.i686 bzip2-libs.i686

cd /

sudo wget https://redirector.gvt1.com/edgedl/android/studio/ide-zips/2024.2.1.11/android-studio-2024.2.1.11-linux.tar.gz

mkdir ADB_DOWNLOAD

tar -xvzf android-studio-2024.2.1.11-linux.tar.gz -C ADB_DOWNLOAD

cd ADB_DOWNLOAD

cd android-studio/bin

chmod +x ./studio.sh

./studio.sh

apt install winetricks -y

winetricks --self-update -y

mkdir /usr/dwnlds

cd /usr/dwnlds

wget https://get.opera.com/ftp/pub/opera_gx/114.0.5282.159/win/Opera_GX_114.0.5282.159_Setup.exe

wine /usr/dwnlds/Opera_GX_114.0.5282.159_Setup.exe

ifconfig

cd

echo Installation Completed

echo use the IP address shown above and rdp to port 3389 or 3390

echo please read the continuing to auto-enable xrdp

echo to run Android Studio run cd /usr/adb/android-studio/bin && ./studio.sh

echo on powershell run wsl --shutdown & wsl.exe


ifconfig

echo Installation Completed

echo use the IP address shown above and rdp to port 3389 or 3390

echo please read the continuing to auto-enable xrdp

echo some packages are not installed... look at the WSL_Lynix.txt file to do a complete install



STOP COPYING FROM HERE (THIS IS IMPORTIANT)

Finish the setup in Android Studio

When your in Android Studio, Click the setting icon and choose "Create Desktop Entry" and choose "create the entry for all users ((requires superuser privillages))

______________________________________________________Fix xRDP___

Reboot your WSL by going to powershell

wsl.exe --shutdown

wsl.exe

________________________________________________XFCE4____________

In here we have to start xfce4 when the pc starts... to do so go to your ubuntu terminal and type

sudo nano /etc/xrdp/startwm.sh

**copy the last 4 codes in to the startwm.sh file***

#test -x /etc/X11/Xsession && exec /etc/X11/Xsession

#exec /bin/sh /etc/X11/Xsession

startxfce4

and it should look like

![Screenshot 2024-11-09 125340](https://github.com/user-attachments/assets/438363ee-3705-4f56-8a68-c57c17261337)

Then exit by pressing (esc) and then (:q) (enter)

startxfce4




___________________________________TRY VISUAL STUDIO CODE__________
Now open a new terminal of ubuntu and type type

code

When prompted enter (Y)



________________________________________________TEST_______________
After the installation with these apps Open file explorer and go to this location

%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Ubuntu

And now press (Windows + R) and type mstsc 
Go back to the Ubuntu terminal and type 

________________________________________________RDP________________

ifconfig

this is what it should look like

eth0: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500

        inet 172.26.203.xxx  netmask 255.255.240.0  broadcast 172.26.207.255
        
        inet6 fe80::215:5dff:fe41:16b7  prefixlen 64  scopeid 0x20<link>![image_2024-11-09_125443717](https://github.com/user-attachments/assets/f9bdafb7-537e-4b9e-8d31-bd546b32c360)


        
        ether 00:15:5d:41:16:b7  txqueuelen 1000  (Ethernet)
        
        RX packets 80062  bytes 131540988 (131.5 MB)
        
        RX errors 0  dropped 0  overruns 0  frame 0
        
        TX packets 8367  bytes 891242 (891.2 KB)
        
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536

        inet 127.0.0.1  netmask 255.0.0.0
        
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        
        loop  txqueuelen 1000  (Local Loopback)
        
        RX packets 1154  bytes 138610 (138.6 KB)
        
        RX errors 0  dropped 0  overruns 0  frame 0
        
        TX packets 1154  bytes 138610 (138.6 KB)
        
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

Now on mstsc type 
iP (use eth0 on linux) - 172.26.203.xxx:xxxx
The port could be 3389,3390, or no port
Username - Not Specified (blank)

Logins

root - *password from line 109* - Xfce4

*unixusername* - *unixpasswd* - Xfce4
________WRAP UP______________________
back in mstsc choose the show options & Connections Settings

Choose Save as and save it in the Lynixity Folder!

___OPTIONAL - RDP FROM ANYWHERE WITH GOOGLE RDP____

So this is optional but IF you need the computer for anywhere or its a server... We need to (optionally) make it usable

1. Goto https://remotedesktop.google.com/access/ on the host (if the host is a server, continue on client)
2. Select "Setup via SSH"
3. Select "Begin"
4. Skip the download
5. Choose Debain linux and copy the command

Enter this on your cmd

wget https://dl.google.com/linux/direct/chrome-remote-desktop_current_amd64.deb
      
the command from Google CRD

Then at the end change it to (WSL) instead of (hostname)

Thats it!
