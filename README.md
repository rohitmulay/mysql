# mysql
<h2> MySQL Installation Procedure for Linux </h2>
First, make sure that your terminal has access to the internet. (If you are using a Proxy network please visit https://github.com/rohitmulay/setproxy )

Then, Update and Upgrade using the following commands: 

`sudo apt-get update`        # Fetches the list of available updates

`sudo apt-get upgrade`       # Strictly upgrades the current packages

`sudo apt-get dist-upgrade`  # Installs updates (new ones)

Open the terminal and give the following command: 
`sudo apt-get install mysql-server` and press enter. 

If you get the following Error: 

    E: Could not get lock /var/lib/dpkg/lock - open (11 Resource temporarily unavailable)
    E: Unable to lock the administration directory (/var/lib/dpkg/) is another process using it?  
    
You can delete the lock file with the following command:

`sudo rm /var/lib/apt/lists/lock`

You may also need to delete the lock file in the cache directory

`sudo rm /var/cache/apt/archives/lock`

`sudo rm /var/lib/dpkg/lock`

After this, close the terminal and open again.

Give the following command: 
`sudo apt-get install mysql-server` and press enter. 
MySQL should install now! 

You will get a prompt asking to download via internet `Do you want to continue? Y/N`

Type `Y` and press enter. 

After installation a dialoge box will open to set the root password.
<img src="https://image.ibb.co/fiG2P5/mysql1.png" alt="mysql1" border="0"> 

Set the password as `root123` or anything you like and press OK. 

Repeat the same Password again in the next dialog box and press enter. 

Installation completed! Now you are good to use MySQL on your system.
