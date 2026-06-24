# Discription
- This repo is used to install software in a new Ubuntu machine

# Instructions
- coppy repo into Ubuntu machine; `git clone https://github.com/DanOlinski/installpack.git`
- make file executable: 
    - go into repo folder 
    - run the command: `chmod u+x installpack1.sh` and `chmod u+x installpack2.sh`
- run the file: `./installpack1.sh`
- restart terminal
- run the file: `./installpack2.sh`

- Finish setting up Postgress
    - type; `sudo -u postgres psql postgres`
    - set a password for a database after typing psql(as above); `\password postgres` (press enter and type your password. suggested pw = pass)
    - type `\q` to get out of postgress interface

# Check if everything was installed
- apache: `sudo systemctl status apache2`
- node:
    - `nvm -v`
    - `node -v` (to change node to another version: nvm use v16)
    - `npm -v`
    - `nvm ls` shows you all the versions installed

# Set AWS permissions
- if you are runing a server in AWS; 
    - go to security rules, edit inbound rules and add a rule
    - the type of rule should be Custom TCP
    - range port is whatever port you are serving at, example 8001
    - add permission to all IP adresses to access the site: 0.0.0.0/0
    - find the served website by navigating to a URL that looks like this: http://3.135.190.22:8001/

- to start an ExpressJs server run the following, from the src folder; `pm2 start index.js` or `pm2 start server.js` (`pm2 stop all`)
- to start a react app; `screen -d -m npm start`