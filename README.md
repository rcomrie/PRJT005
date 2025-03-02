Project: Automated Linux System Update Script

Project Detail : This script will Update and upgrade system packages and log the update process.

Project Description"

step-1  Create the Bash Script

vi update.sh

#/!bin/bash
sudo yum  update
sudo yum  upgrade




step-2 Grant Execute Permission

chmod 777 update.sh



step-3  Run the Script

./update.sh


====================================

Project: Automated Linux System install and start httpd services through Script


vi system.sh

#!/bin/bash
systemctl start httpd
systemctl status httpd

chmod 777 system.sh
./system.sh


-------------------------------------------------

vi httpd.sh

#!/bin/bash
yum install httpd -y
systemctl start httpd
systemctl status httpd

chmod 777 httpd.sh
./httpd.sh

---------------------------------------------------

vi remove.sh

#!/bin/bash
yum remove httpd -y

chmod 777 remove.sh
./remove.sh

-------------------------------------------------------

vi docker.sh

#!/bin/bash
yum install docker -y
systemctl start docker
systemctl status docker

chmod 777 docker.sh
./docker.sh


--------------------------------------------------------

git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/rcomrie/PRJT005.git
git push -u origin main

git config --global user.name "rcomrie"
git config --global user.email "rojaecomrie@gmail.com"

