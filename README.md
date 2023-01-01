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
wget https://chromedriver.storage.googleapis.com/108.0.5359.71/chromedriver_linux64.zip

unzip chromedriver_linux64.zip
