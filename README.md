# How to install and Configure

1. New directory on your system
2. vagrant init to launch vagrant
3. clone the mongo file
4. set up read me and gitignore

5. use vagrant up

6. the vagrant ssh to launch

wget -qO - https://www.mongodb.org/static/pgp/server-3.2.asc | sudo apt-key add -

echo "deb http://repo.mongodb.org/apt/ubuntu xenial/mongodb-org/3.2 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-3.2.list

sudo apt-get update

sudo apt-get install -y mongodb-org=3.2.20 mongodb-org-server=3.2.20 mongodb-org-shell=3.2.20 mongodb-org-mongos=3.2.20 mongodb-org-tools=3.2.20

# Install the Mongodb Packages

1. Install the latest stable version:
sudo apt-get install -y mongodb-org

# Start Mongodb
sudo service mongod start

# Verify that is has started successfully
sudo service mongod status

# To Stop MongoDB
sudo service mongod stop

# To Restart it
sudo service mongod restart

# Begin using MongoDB
mongo

#To enable mongod
sudo systemectl enable mongod.service

# How to access the conf file

    sudo nano /etc/mongod.conf
