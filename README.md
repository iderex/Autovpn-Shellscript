# Description:
Make the script executable "chmod +x /path/to/the/script.sh
Put the script in .profile or .bashrc so it can be run on user login:
Example: echo "/path/to/the/script.sh start &" >> .bashrc
The script can be bound to shortcut keys with these commands:
/path/to/the/script.sh start # starts and monitors VPN connection
/path/to/the/script.sh stop # stops the monitor and also the VPN connection

##########
# Config #
##########

You can see those with "nmcli con show --active" command

VPN_NAME="VPN-NAME-HERE"
VPN_UID="VPN-UID-HERE"

Delay in secconds

DELAY=300

File path with write permission to the executing user to store script status information

LOG="/path/to/log/file.log"

Enable/disable ping connection check

PING_CHECK_ENABLED=true

Check IP/Hostname

CHECK_HOST="8.8.8.8"

Configure DISPLAY variable for desktop notifications

DISPLAY=0.0
