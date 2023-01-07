# Ubuntu-22.10-Things-to-do-after-installation

The following is a list of libraries and tools to improve the over all experience, including replacing the default firefox installation by the Mozilla team PPA source.

# Enable fingerprint security
- sudo apt remove fprintd
- sudo add-apt-repository ppa:uunicorn/open-fprintd 	
- sudo apt install open-fprintd fprintd-clients python3-validity 	
- fprintd-enroll <User> 	
- sudo pam-auth-update 	

# Ubuntu libraries and extras
- sudo apt-get update 
- sudo apt install ubuntu-restricted-extras 	
- sudo apt install libfuse2 	
- sudo apt install flatpak 	
- sudo apt install chrome-gnome-shell 	
- sudo apt install dconf-editor 	
- sudo apt install gnome-tweaks 	
- sudo apt install gnome-shell-extension-manager
# Install Mozilla team firefox
# If installes first remove firefox from the system
- sudo apt remove firefox 	
- sudo snap remove --purge firefox
# Add the repository for Mozilla Team
- sudo add-apt-repository ppa:mozillateam/ppa 	
- sudo nano /etc/apt/preferences.d/99mozillateamppa

- The contents of this file should be:
- Package: firefox*
- Pin: release o=LP-PPA-mozillateam
- Pin-Priority: 501

- Package: firefox*
- Pin: release o=Ubuntu
- Pin-Priority: -1

- Save and exit the file then 

- sudo apt update 	
- sudo apt install firefox
