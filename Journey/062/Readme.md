

# Deploying OpenLiteSpeed on EC2

## Cloud Research

**Creating EC2 Instance by following details**
- AMI Ubuntu 20.04
- Enabling Public IP
- Using pem. for primary key so that it can be SSH through Putty

**Deploying OpenLiteSpeed**
- SSH through Putty
- Running following commands based on https://www.howtoforge.com/tutorial/how-to-install-and-configure-openlitespeed-server-along-with-mariadb-and-php-on-ubuntu-2004/

Update system.

$ sudo apt update

$ sudo apt upgrade

Step 1 - Configure Firewall

We need to enable SSH, HTTP, HTTPS and ports 7080, 8088 for the firewall.

$ sudo ufw allow OpenSSH

$ sudo ufw allow http

$ sudo ufw allow https

$ sudo ufw allow 7080/tcp

$ sudo ufw allow 8088/tcp

Check the status of the firewall.

<image src= https://user-images.githubusercontent.com/99172259/171991635-052aa205-8bbf-4c7a-bb20-43d0acdd42e0.png width="450" height="300" />

Step 2 

Add the OpenLiteSpeed Repository Key.

$ wget -qO - https://rpms.litespeedtech.com/debian/lst_repo.gpg | sudo apt-key add -

Add the Repository.

$ echo "deb http://rpms.litespeedtech.com/debian/ focal main" | sudo tee /etc/apt/sources.list.d/openlitespeed.list

Update the Repository.

$ sudo apt update

Install OpenLiteSpeed

$ sudo apt install openlitespeed

Check the status of the server.

$ sudo /usr/local/lsws/bin/lswsctrl status

Step 3 - Configure OpenLiteSpeed

$ sudo /usr/local/lsws/admin/misc/admpass.sh

## ☁️ Cloud Outcome

Here is the result after I enter the front page of the web server http://54.237.46.73:8088/

<img src= https://user-images.githubusercontent.com/99172259/171991824-10ab37cd-36c6-476f-93d4-346c6ad59861.png width="450" height="300" />

Here is the admin panel

<img src= https://user-images.githubusercontent.com/99172259/171991911-20cad3f2-dfba-4faf-8592-4839b2f099c4.png width="450" height="300" />


## Social Proof


[Twitter](https://twitter.com/JoeSeven08/status/1533008703850696704)
