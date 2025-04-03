# Earn Grass Coins on Raspberry Pi for passive Earnings
If you’re looking for a way to passively earn Grass Coins using your Raspberry Pi, this guide will walk you through every step. I personally tested this method on my Raspberry Pi and found it to be stable and efficient.

Initially, I attempted to install the GetGrass Desktop Version for Linux, which offers a 2x points boost, but unfortunately, it failed to work on my setup. As a result, I opted for the Grass Community Extension on Chromium, which operates at a 1.25x boost. Despite this, the setup runs smoothly with an average temperature of 55°C—even without passive or active cooling. I run my grass node on a Raspberry Pi 3+ 1GB

**💡 Before You Start:**

To begin earning, you’ll need an account on GetGrass.io. If you want to support me you can use or share my referral link (you'll earn 5000 after 100hrs of uptime) - [https://app.getgrass.io/register/?referralCode=4x856vcOc8W1nXm](https://app.getgrass.io/register/?referralCode=4x856vcOc8W1nXm)

# Step 1: Install Raspberry Pi Imager

First, download and install Raspberry Pi Imager on your computer. This tool makes it easy to set up Raspberry Pi OS (64-bit) on an SD card. I use a 32GB but a 16GB should also work

1. [Download Raspberry Pi Imager](https://www.raspberrypi.com/software/)
2. Install it on Windows, macOS, or Linux.



# Step 2: Create a Raspberry Pi OS 64-Bit Image

1. Open Raspberry Pi Imager.
2. Click “Choose OS” → Select Raspberry Pi OS (64-bit).
3. Click “Choose Storage” → Select your SD Card (minimum 16GB recommended).
4. Click “Write” to create the bootable image.
5. Wait until the process completes, then eject the SD card.

# Step 3: Boot into Raspberry Pi OS

1. Insert the SD card into your Raspberry Pi.
2. Connect power, a keyboard, a mouse, and a monitor.
3. The system will boot into Raspberry Pi OS 64-bit.
4. Follow the setup instructions (WiFi, updates, etc.).

# Step 4: Enable Developer Mode in Chromium

1. Open Chromium on your Raspberry Pi.
2. In the address bar, type chrome://extensions/ and press Enter.
3. Toggle Developer Mode to ON (top right corner).

# Step 5: Download & Install Grass Community Extension

Since the Grass Desktop Version did not work for me, I used the Grass Community Extension, which runs smoothly and provides 1.25x earnings boost.

1. Go to the Grass Store ([https://app.getgrass.io/dashboard/store/item/extension/install](https://app.getgrass.io/dashboard/store/item/extension/install)).
2. Download the Grass Community Extension for Linux.
3. Locate the downloaded .zip file.
4. Unzip the file and find the .crx extension file.

# Step 6: Install the Extension in Chromium

1. Open Chromium and go to chrome://extensions/.
2. Drag and drop the unpacked .crx file into the Extensions page.
3. When prompted, click “Add Extension” to confirm.

# Step 7: Pin the Extension for Easy Access

1. Click the puzzle piece icon in the upper right corner of Chromium.
2. Scroll down to Grass Community Extension.
3. Click the pin icon to add it to the toolbar.

# Step 8: Log In and Start Earning

1. Visit [app.getgrass.io](http://app.getgrass.io) and log in to your Grass account.
2. The extension will now start passively earning points.
3. Keep your Raspberry Pi powered on to maximize uptime and earnings.



# Performance and Stability

After running this setup for several weeks, I can confirm that it works stably on the Raspberry Pi. The device maintains an average temperature of 55-65°C without any passive or active cooling. With cooling the average temperature ist between 45-55°C. This means you can safely leave your Raspberry Pi running 24/7 without worrying about overheating.



# Pro Tip: Launch Chromium on startup

If you want to launch Chromium on startup just modify the Exec line in your chromium.desktop file:

1. Open a terminal & run 
```
mkdir -p ~/.config/autostart"
```
2. Create a .desktop file with: 
```
nano ~/.config/autostart/chromium.desktop
```
3. Paste the following:
```
[Desktop Entry]
Type=Application
Exec=chromium-browser
Hidden=false
NoDisplay=false
X-GNOME-Autostart-enabled=true
Name=Chromium
Comment=Start Chromium on login
```
4. Save and exit (Ctrl+O, then Enter, then Ctrl+X)
5. to reboot the system to check if chormium lunches on startup run
```
sudo reboot
```


# Maximizing Earnings: Other Passive Income Nodes on Raspberry Pi

Since the Raspberry Pi is already running Chromium, you can also install additional passive income nodes to maximize your earnings. Here are a few other nodes I personally run on my Raspberry Pi:

1. Gradient Network – AI computing power sharing (🔗 [Join Gradient Network](https://app.gradient.network/signup?code=ZQSJY6))
2. Nodepay – Passive income through decentralized financial services (🔗 [Join Nodepay](https://app.nodepay.ai/register?ref=NDUvP8Rlp5dPyNq))
3. Bless Network – Decentralized network rewards (🔗 [Join Bless Network](https://bless.network/dashboard?ref=973E48))
4. MystNodes Network – Open Web Protocol (🔗 [Get a 5% Bonus in your first Month](https://mystnodes.co/?referral_code=BUmKWB7kB6eiejJETzeSbglOId0Lp3etFY8xkaAK))

Read this to setup the MystNode on your Pi:

1. [Updating your node](https://help.mystnodes.com/en/articles/8006202-raspberry-pi-guide) 
(After "Install a Mysterium node" you won't be able to access the internet becasue resolving the IP is not working. To fix it, use
```
sudo cat /etc/resolv.conf && sudo resolvconf -u
```
2. To check if the Node i running check this commands [Installing a Mysterium node using install script](https://help.mystnodes.com/en/articles/4531779-installing-a-mysterium-node-using-install-script)



# Final Thoughts

If you’re looking for a low-power, passive income setup, running the Grass Community Extension on Raspberry Pi is a great option. While the Linux Desktop Version didn’t work for me, this Chromium-based method is a reliable alternative.

Since Chromium is already running, you can install multiple nodes to diversify your passive income. If you’re interested in earning more, consider adding the Gradient Network, Nodepay, Bless Network and MystNodes Network to your setup.

💰 Happy earning! 🚀
