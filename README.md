# DonorsChoose_Visualization
* Source Code for my blog post: [Interactive Data Visualization with D3.js, DC.js, Python, and MongoDB](http://adilmoujahid.com/posts/2015/01/interactive-data-visualization-d3-dc-python-mongodb/)

#Visit my Blog : http://adilmoujahid.com

## Getting started

The dependencies for the project can be installed using

    $ pip install -r requirements.txt

You can use ``Vagrant`` to start a machine with a MongoDB instance running

    $ vagrant up

To initialize the database you need to download the data

    $ wget https://s3.amazonaws.com/open_data/csv/opendata_projects.zip && unzip opendata_projects.zip

and import it

    $ mongoimport -d donorschoose -c projects --type csv --file /vagrant/opendata_projects.csv -headerline

# by Yan from:
https://www.tutorialspoint.com/mongodb/mongodb_environment.htm

Install MongoDB on Ubuntu
Run the following command to import the MongoDB public GPG key −

sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv 7F0CEB10
Create a /etc/apt/sources.list.d/mongodb.list file using the following command.

echo 'deb http://downloads-distro.mongodb.org/repo/ubuntu-upstart dist 10gen' 
   | sudo tee /etc/apt/sources.list.d/mongodb.list
Now issue the following command to update the repository −

sudo apt-get update
Next install the MongoDB by using the following command −

apt-get install mongodb-10gen = 2.2.3
In the above installation, 2.2.3 is currently released MongoDB version. Make sure to install the latest version always. Now MongoDB is installed successfully.

Start MongoDB
sudo service mongodb start
Stop MongoDB
sudo service mongodb stop
Restart MongoDB
sudo service mongodb restart
To use MongoDB run the following command.

mongo
