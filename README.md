# system-startup-essentials
```bash
sudo apt-get update && apt upgrade -y
sudo apt-get install network-manager -y
sudo apt-get install ntp -y
sudo systemctl start ntp
sudo systemctl enable ntp
```

This script updates the package lists for upgrades for all installed packages, upgrades them, installs the NetworkManager package, installs the NTP package, starts the NTP service, and enables it to start automatically on system boot. Here's a breakdown:

1. `sudo apt-get update`: This updates the package lists for upgrades for all installed packages.

2. `apt upgrade -y`: This command upgrades all the installed packages. The `-y` flag is used to automatically answer "yes" to all prompts during the upgrade process.

3. `sudo apt-get install network-manager -y`: This installs the NetworkManager package, which is used for managing network connections.

4. `sudo apt-get install ntp -y`: This installs the NTP (Network Time Protocol) package, which is used for time synchronization.

5. `sudo systemctl start ntp`: This starts the NTP service.

6. `sudo systemctl enable ntp`: This enables the NTP service to start automatically on system boot.

This script is useful for ensuring that the system is up-to-date, has network management capabilities, and is synchronized with an NTP server for accurate timekeeping.
