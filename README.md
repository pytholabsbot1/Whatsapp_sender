# Whatsapp_sender

System Config : Ubuntu 20.14 LTS


# Add user
sudo adduser vaqas
sudo adduser vaqas sudo

sudo ufw enable
sudo ufw allow OpenSSH
sudo ufw allow 9000
sudo ufw allow 8000


export PATH="/home/ubuntu/.local/bin:$PATH"
mkdir wa_sender
cd wa_sender

# Update and shit
sudo apt-get update && sudo apt-get upgrade 

sudo apt-get install python3-pip tmux htop snapd -y

pip3 install selenium==3.141.0 flask jupyter notebook
jupyter notebook --ip=0.0.0.0 --port=8000
flask run --host=0.0.0.0 --port=9000

# Get Chrome

To install Chrome on Ubuntu server from the terminal, follow these steps:

wget https://dl.google.com/linux/linux_signing_key.pub
sudo apt-key add linux_signing_key.pub
sudo sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
sudo apt-get update
sudo apt-get install google-chrome-stable

wget https://chromedriver.storage.googleapis.com/108.0.5359.71/chromedriver_linux64.zip

unzip chromedriver_linux64.zip
