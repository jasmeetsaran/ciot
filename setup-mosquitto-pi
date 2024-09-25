Update Raspberry Pi
-----------------------------------------------------------------
sudo apt update
sudo apt full-upgrade -y


Install Mosquitto Broker
-----------------------------------------------------------------
sudo apt install mosquitto mosquitto-clients -y


Create Mosquitto service & check installation
-----------------------------------------------------------------
sudo systemctl enable mosquitto.service

mosquitto -v


Enable Remote Access
-----------------------------------------------------------------
Edit mosquitto.conf
sudo nano /etc/mosquitto/mosquitto.conf


add this as first line
-----------------------------------------------------------------
per_listener_settings true


add this to end
-----------------------------------------------------------------
allow_anonymous false 
listener 1883  
password_file /etc/mosquitto/passwd


Your configuration file will look like
-----------------------------------------------------------------
# Place your local configuration in /etc/mosquitto/conf.d/
#
# A full description of the configuration file is at
# /usr/share/doc/mosquitto/examples/mosquitto.conf.example

per_listener_settings true

pid_file /run/mosquitto/mosquitto.pid

persistence true
persistence_location /var/lib/mosquitto/

log_dest file /var/log/mosquitto/mosquitto.log

include_dir /etc/mosquitto/conf.d
allow_anonymous false 
listener 1883  
password_file /etc/mosquitto/passwd
-----------------------------------------------------------------


Create password file
-----------------------------------------------------------------
sudo touch /etc/mosquitto/passwd


Create password for user
-----------------------------------------------------------------
sudo mosquitto_passwd /etc/mosquitto/passwd user

Enter password twice to set


Restart Mosquitto
-----------------------------------------------------------------
sudo systemctl restart mosquitto

Check status
-----------------------------------------------------------------
sudo systemctl status mosquitto


MQTT X download link
-----------------------------------------------------------------
https://mqttx.app/
