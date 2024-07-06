## Update and Upgrade The System:

```md	
sudo apt update
```

```md	
sudo apt upgrade
```

## GUI if needed:

### Install gdm3

```md
sudo apt install gdm3
```

### Install xfce4 xfce4-goodies

```md	
sudo apt install xfce4 xfce4-goodies -y
```

## xrdp:
### Install xrdp

```md	
sudo apt install xrdp -y
```

### Check for Status xrdp

```md	
sudo systemctl status xrdp
```

### Configure gui

```md	
sudo update-alternatives --config x-session-manager
```

> set to startxfce4

### for more configration:

```md	
sudo nano /etc/xrdp/xrdp.ini
```

## ufw:
### configure ufw

```md	
sudo ufw allow from [IP_LOCAL]/32 to any port 3389
```
> [IP_LOCAL] for the Client device, "in this Step I did The local ip not the public, I hope it's ez XD"

### Check Changes in ufw

```md	
sudo ufw status
```

### If It's inactive

```md	
sudo ufw enable
```

## References:
- TUTORIAL How To Enable Remote Desktop Protocol Using xrdp on Ubuntu 22.04 Published on September 20, 2022 (Raghav Aggarwal and Caitlin Postal) <a href="https://www.digitalocean.com/community/tutorials/how-to-enable-remote-desktop-protocol-using-xrdp-on-ubuntu-22-04#step-3-configuring-xrdp-and-updating-your-firewall">Link</a>
- askubuntu ""Oh no! Something has gone wrong" / ubuntu 23.04 / xrdp / xfce-desktop / Google Compute" answered Jun 28, 2023 at 11:37 (Avamander) <a href="https://askubuntu.com/questions/1475045/oh-no-something-has-gone-wrong-ubuntu-23-04-xrdp-xfce-desktop-google">Link</a>



