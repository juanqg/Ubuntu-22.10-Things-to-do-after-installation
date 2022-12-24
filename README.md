# Ubuntu-22.10-Things-to-do-after-installation

The following is just a list of commands to improve the over all experience

# Enable fingerprint security
sudo apt remove fprintd
sudo add-apt-repository ppa:uunicorn/open-fprintd 	
sudo apt install open-fprintd fprintd-clients python3-validity 	
fprintd-enroll <User> 	
sudo pam-auth-update 	

# Ubuntu libraries and extras
sudo apt-get update 
sudo apt install ubuntu-restricted-extras 	
sudo apt install libfuse2 	
sudo apt install flatpak 	
sudo apt install chrome-gnome-shell 	
sudo apt install dconf-editor 	
sudo apt install gnome-tweaks 	
sudo apt install gnome-shell-extension-manager 	
sudo apt remove firefox 	
sudo snap remove --purge firefox 	
sudo add-apt-repository ppa:mozillateam/ppa 	
sudo nano /etc/apt/preferences.d/99mozillateamppa
sudo apt update 	
sudo apt install firefox
