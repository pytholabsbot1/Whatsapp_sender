# Whatsapp_sender

System Config : Ubuntu 20.14 LTS


# Add user
sudo adduser vaqas
sudo adduser vaqas sudo

export PATH="/home/vaqas/.local/bin:$PATH"
mkdir wa_sender
cd wa_sender

# Update and shit
sudo apt-get update && sudo apt-get upgrade 

sudo apt-get install python3-pip chromium tmux htop -y

pip3 install selenium jupyter notebook


# Get Chrome
wget https://chromedriver.storage.googleapis.com/105.0.5195.52/chromedriver_linux64.zip

unzip chromedriver_linux64.zip
