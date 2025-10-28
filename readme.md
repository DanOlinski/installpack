# Discription
- This repo is used to install software in a new Ubuntu machine

# Instructions
- coppy repo into Ubuntu machine
- make file executable: 
    - go into repo folder 
    - run the command: `chmod u+x installpack1.sh` and `chmod u+x installpack2.sh`
- run the file: `./installpack1.sh`
- restart terminal
- run the file: `./installpack2.sh`

- Finish setting up Postgress
    - type; `sudo -u postgres psql postgres`
    - set a password for a database after typing psql(as above); `\password postgres` (press enter and type your password. suggested pw = pass)

# Check if everything was installed
- apache: `sudo systemctl status apache2`
- node:
    - `nvm -v`
    - `node -v` (to change node to another version: nvm use v16)
    - `npm -v`
    - `nvm ls` shows you all the versions installed