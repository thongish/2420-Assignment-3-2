# 2420-Assignment-3-2

# Setting up a load balancer on DigitalOcean

>[!NOTE]
> When making your droplets, give them identical tags. This will be used later on when we create the load balancer.

Set up two identical Nginx web server droplets on your DigitalOcean account using the files and script in this repository. Follow the steps below:

1. First thing you need to do is ensure your droplets Arch Linux system is up-to-date:
```
sudo pacman -Syu
```

2. Make sure to reboot the droplet as well:
```
sudo reboot
```
>[!NOTE]
> This will kick you out of your server. It will take a minute or so until you can SSH back in.

3. SSH back into your droplet and clone this repository into your home directory:
```
git clone https://github.com/thongish/2420-Assignment-3-1.git ~/nginx-setup
```

4. cd into the cloned directory:
```
cd ~/nginx-setup
```

5. Run the script with this command:
```
sudo ./setup-script
```

Check that everything worked by entering your both your droplet's IP addresses in your web browser. You should see something like this:

![Screenshot of working Nginx web server](./assets/success.png)
