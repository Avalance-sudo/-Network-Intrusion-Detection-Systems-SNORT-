ifconfig  # Check the network interfaces (looking for eth0,enp0s3,etc.)
snort -V   #Verify Snort is installed 

#Update the system on Ubuntu 
sudo apt-get update && sudo apt-get dist-upgrade -y # Edit Snort main congiguration 
sudo gedit/etc/snort/rules/ftp. rules # Create or edit custom FTP rule 
sudo snort -T -c /etc/snort/snort.cong -i eth0
sudo snort -A console -q 0u snort -g snort -c /etc/snort/snort.conf -i eth0 

# For the Kail machine
namp 192.168.1.xx # Replace with Ubuntu machine's Ip address

# you should see alers in the snort teminal if everything is set up correctly
[**] [1:1000003:1] FTP connection detected [**]

# if nothing show up,try using a more gerneal rule in local.rule
alert ip any any -> any any (msg:"Generic IP Packet Detected"; sid:1000001; rev:1;)
