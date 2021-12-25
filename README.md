Command to install

wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash && export NVM_DIR="$HOME/.nvm" && [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" && [ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion" && nvm install 16 && apt install git -y && git clone https://github.com/Penguinehis/dragoncheckbeta.git && cd dragoncheckbeta && npm i && screen -dmS api node index.js TOKEN

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
