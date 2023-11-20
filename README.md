# PiHole-Setup-RaspberryPi

<p align="center">
  <img src="https://elinux.org/images/c/cb/Raspberry_Pi_Logo.svg" width="25%" />
  <img src="https://i0.wp.com/pi-hole.net/wp-content/uploads/2016/07/Pi-hole-vortex2.jpg" width="25%" />
</p>

A comprehensive guide for setting up Pi-hole on a Raspberry Pi. This repository provides step-by-step instructions, from initial Raspberry Pi setup to Pi-hole configuration, ensuring a smooth installation process for users of all skill levels. It includes detailed explanations of each step, troubleshooting tips, and links to essential resources. Perfect for beginners looking to create an efficient network-wide ad blocker.

### What You Need
1. **Raspberry Pi**: With a compatible OS installed (Raspberry Pi OS is recommended).
2. **Internet Connection**: Wired or wireless.
3. **Power Supply**: For your Raspberry Pi.
4. **Micro SD Card**: With the OS installed.
5. **Computer**: To access the Raspberry Pi remotely.
6. **SSH Client**: Like PuTTY for Windows or Terminal for macOS/Linux.

### Step 1: Update and Upgrade Raspberry Pi OS
First, ensure your Raspberry Pi is up to date:
- Open the Terminal on Raspberry Pi.
- Type `sudo apt update` and press Enter.
- After it finishes, type `sudo apt upgrade` and press Enter.
- Reboot if necessary.

### Step 2: Install Pi-hole
- In the Terminal, type `curl -sSL https://install.pi-hole.net | bash` and press Enter.
- Follow the on-screen instructions to complete the installation.

### Step 3: Configure Pi-hole
- After installation, Pi-hole will display an IP address and a password for the admin web interface.
- Note these down.
- Access the admin interface by typing the IP address into a web browser from any device on your network.

### Step 4: Setting Up DNS
- Log into your router's admin page (usually something like 192.168.0.1 or 192.168.1.1).
- Locate the DNS settings.
- Change the DNS server to the IP address of your Raspberry Pi.
- Save and restart your router.

### Step 5: Accessing the Pi-hole Dashboard
- Open a web browser and enter `http://[your Pi's IP address]/admin`.
- Log in using the password generated during the installation.

### Step 6: Configuring Blocklists
- In the Pi-hole dashboard, go to 'Settings' > 'Blocklists'.
- Add or remove lists as per your preference.

### Step 7: Updating Pi-hole
- Regularly update Pi-hole by typing `pihole -up` in the Terminal.

### Tips for Troubleshooting
- If you encounter issues, rebooting your Raspberry Pi and router can resolve many problems.
- Check the Pi-hole community forums and FAQs for specific issues.

### Additional Resources
- [Pi-hole Official Website](https://pi-hole.net/)
- [Raspberry Pi OS Download](https://www.raspberrypi.org/downloads/)
- [Pi-hole Installation Guide](https://docs.pi-hole.net/main/basic-install/)
- [Pi-hole Forums](https://discourse.pi-hole.net/)

### Safety and Security
- Regularly update your Raspberry Pi OS and Pi-hole for security.
- Consider setting up a firewall on your Raspberry Pi.
