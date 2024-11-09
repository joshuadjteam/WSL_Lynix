Hello guys!

Here at DJTeam we've been working on Lynix to Linux (Work in progress with WSL) and its a sucess!
To Buy the New version (1.2.1a) goto https://lynixity.x10.bz/

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

apt update && apt upgrade

sudo snap install firefox

sudo apt install x11-apps -y

sudo apt install ubuntu-desktop

apt install xfce4 xfce4-goodies && echo On xfce4 choose gdm3 when prompted

apt install xrdp -y

echo "xfce4-session" | tee .xsession

systemctl restart xrdp

sudo apt install gedit -y

sudo apt install gimp -y

sudo apt install nautilus -y

sudo apt install vlc -y

cd /tmp

sudo wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.de

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

code

passwd root

ifconfig

STOP COPYING FROM HERE (THIS IS IMPORTIANT)

In here we have to start xfce4 when the pc starts... to do so go to your ubuntu terminal and type

sudo nano /etc/xrdp/startwm.sh

copy the last 4 codes in to the startwm.sh file

#test -x /etc/X11/Xsession && exec /etc/X11/Xsession
#exec /bin/sh /etc/X11/Xsession

startxfce4

and it should look like

![Screenshot 2024-11-09 125340](https://github.com/user-attachments/assets/438363ee-3705-4f56-8a68-c57c17261337)

TRY VISUAL STUDIO CODE
Now open a new terminal of ubuntu and type type

code

When prompted enter (Y)



TEST
After the installation with these apps Open file explorer and go to this location

%USERPROFILE%\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Ubuntu

And now press (Windows + R) and type mstsc 
Go back to the Ubuntu terminal and type ifconfig

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

root - *password from line 81* - Xfce4

*unixusername* - *unixpasswd* - Ubuntu Desktop

Rdp

when you need to RDP to Ubuntu you can use Lynix
back in mstsc choose the show options & Connections Settings
Choose Save as and save it in the Lynixity Folder!

Thats it!
