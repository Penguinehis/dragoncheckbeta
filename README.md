# Command to install

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash && export NVM_DIR="$HOME/.nvm" && [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" && [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion" && nvm install 16 && apt install git -y && git clone https://github.com/Penguinehis/dragoncheckbeta.git && cd dragoncheckbeta && npm i && screen -dmS api node v12.js --token=TOKEN --port=6888

IN TOKEN, change to your key exemple: penguinehhis091m31041kl4014 (this key not work is just a exemple)

if you view in the command:

 lsof -i :6888 && lsof -i :6889 && lsof -i :8989 && lsof -i :2095 && lsof -i :2096 

the node and the port exemple:

COMMAND    PID USER   FD   TYPE  DEVICE SIZE/OFF NODE NAME<br>
node    794754 root   22u  IPv6 2872037      0t0  TCP *:6888 (LISTEN)

If not try to run the node without the screen to get the error:

node index.js TOKEN

In this case in the folder dragoncheckbeta

If need any support just send a menssage here in github our in the telegram https://t.me/sisudragon


# Restart API After REBOOT:

V12:

cd dragoncheckbeta && screen -dmS api node v12.js --token=TOKEN --port=PORT && cd


# Update to v12:

cd dragoncheckbeta && wget https://raw.githubusercontent.com/Penguinehis/dragoncheckbeta/main/v12.js


# How to auto start with reboot?

in the folder dragoncheckbeta create a .sh with that

#!/bin/bash
screen -dmS api /root/.nvm/versions/node/v16.13.1/bin/node /root/dragoncheckbeta/v12.js --token=TOKEN --port=PORT

Change the Token, to your token

and change the PORT, to your desired port exemple 6888

after that do chmod 777 name of the .sh 

in crontab -e 

select nano

and put this line 

@reboot /root/name of the .sh

ctrl + x

Y 

Enter 

and its it
