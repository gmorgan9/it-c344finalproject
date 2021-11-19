# Project Write up
Garrett Morgan <br/>
November 18th, 2021<br/>
IT&C 344 - Operating Systems<br/>
Albert Tay

## Project Description
I decided to do the first project listed on Alberts list of projects. I had to show how an Apache2 HTTP server works on a linux system and demonstrate a working website from my raspberry pi.

## Team Members Contribution
I ended up completing the final project alone. I was not able to find a group of people in our class to do a project.

## Supplies
### Equipment
- Raspberry Pi 3 B+
- 32gb SD Card
- Ethernet cable
- Monitor
- Macbook Pro
### Software
- Ubuntu Server 21.10 - Installed on raspberry pi
- Raspberry Pi OS Installer - Installed on Macbook Pro to format SD card with Ubuntu Server 21.10
- Visual Studio Code
- Github
- Apache2

## Project Steps
1. I installed the Raspberry Pi OS Installer on my Macbook Pro.
2. 3. I then installed Ubuntu Server 21.10 on my 32gb SD card to place into my Raspberry Pi 3 B+
4. I started up my Raspberry pi and had it connected to one of the monitors in my office in the Marriott School of Business IT office. 
5. I then was able to get all logged into my raspberry pi on Ubuntu.
6. Once I was logged in, I was able to remote into my raspberry pi from my mac using ssh.
7. After getting ssh’ed into my raspberry pi I was able to install apache2 using the command “sudo apt install apache2”
8. After a while, it finally downloaded apache2 on my Raspberry pi and I was able to redirect to my website directory using the command “cd /var/www”
9. I then was able to clone my github that contained my simple website to my website directory on my Raspberry Pi(Ubuntu Server), the command I used to clone my repository is '''git clone [url of git repository]'''.
10. Once I got that cloned, I used the command “sudo service apache2 start” (this command allowed my website to be pushed live on my server).
11. To access my webpage, you just need to be connected to the BYU Eduroam wifi and type in the IP address “10.25.90.143”. You will then see my webpage as shown in the image below.
To take down my website, I used the command “sudo service apache2 stop” (this command will take down my instance of my website from my IP address, so you won’t see it again, so if you went to that IP address after i took it down, it will state that the “Page Not Found”).

