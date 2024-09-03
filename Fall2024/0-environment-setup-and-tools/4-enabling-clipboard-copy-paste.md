# Enabling bi-directional clipboard between your VM and your host

## Windows Hosts and intel Macs
If you are running windows and have already completed the dev envrionment setup assignment, you have already installed guest additions. 

With your VM turned off in VirtualBox go to settings > general > enable the shared clipboard.

## MacOS Hosts 
Open the terminal application in your VM.

Ensure clipboard sharing is enabled in the settings of your VM. 

```
sudo apt install qemu-guest-agent
```
and restart the machine.