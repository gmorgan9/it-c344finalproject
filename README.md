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
2. I then installed Ubuntu Server 21.10 on my 32gb SD card to place into my Raspberry Pi 3 B+
3. I started up my Raspberry pi and had it connected to one of the monitors in my office in the Marriott School of Business IT office. 
4. I then was able to get all logged into my raspberry pi on Ubuntu.
5. Once I was logged in, I was able to remote into my raspberry pi from my mac using ssh.
6. After getting ssh’ed into my raspberry pi I was able to install apache2 using the command `sudo apt install apache2`
7. After a while, it finally downloaded apache2 on my Raspberry pi and I was able to redirect to my website directory using the command `cd /var/www`
8. I then was able to clone my github that contained my simple website to my website directory on my Raspberry Pi(Ubuntu Server), the command I used to clone my repository is `git clone [url of git repository]`
9. Once I got that cloned, I used the command `sudo service apache2 start` (this command allowed my website to be pushed live on my server).
10. To access my webpage, you just need to be connected to the BYU Eduroam wifi and type in the IP address `10.25.90.143`. You will then see my webpage as shown in the image below.
11. To take down my website, I used the command `sudo service apache2 stop` (this command will take down my instance of my website from my IP address, so you won’t see it again, so if you went to that IP address after i took it down, it will state that the `Page Not Found`).

Some other information I would like to share about my project is how I could update my website any time using VS code and what commands I used to update it on my live server. These steps include:
1. I would update my code in VS code how I would like. 
2. I would then commit and push my work to github (this was done in VS code which is linked to my github account).
3. After seeing the changes in my github account, I would go to the terminal and pull the updated files to my apache server. 
4. To pull the updated files over, I would use the command `git pull origin main` (this would pull the updated files from my git repository that was changed in VS code).
5. I then reloaded my apache2 server by using the command `sudo service apache2 restart` (this command would restart the server and show the updated web pages that were updated in VS code).
## Project Questions
- How do you install apache2 (What commands did you use?)
- - How do you install apache2 (What commands did you use?)
