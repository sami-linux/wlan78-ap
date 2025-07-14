# Linux Wi-Fi Access Point : wlan78-ap
- So far, This script has been tested on Debian and distributions based on it, ubuntu and distributions based on it, Linux Mint, Gentoo, Manjaro, archlinux, Fedora, Calculate Linux and Sysrescuecd. I'll add the tested distributions progressively.
- If your interface refuses to reconnect, which is rare, immediately run "./wlan78-ap reset". Everything will return to normal, and you can      then reactivate your access point with confidence by running "./wlan78-ap".
## 📌 Why, this script?

- **Windows provides a built-in graphical tool** to create a Wi-Fi hotspot — but Linux does not.
- This project offers a **simple way** to create a functional access point from any Linux system **without complex config files**.
- This script is especially designed for people who don't have Ethernet access and want to use their Linux system as a Wi-Fi repeater of       their existing Wi-Fi network.
- No need to touch any config file — everything is generated dynamically.

## ✅ Features

- Automatically detects a Wi-Fi interface connected to the Internet.
- Dynamically generates all necessary configuration files.
- Creates a virtual access point (`wlan78`) in seconds.
- Just type a password, and the AP is ready.
- Run `wlan78-ap reset` anytime to **reset and start clean** 

## 🧱 Requirements

Make sure your Wi-Fi interface supports AP mode (Access Point). It must be capable of acting as both a client (to get Internet) and a server (to share it) simultaneously.

Make sure the following tools are installed:

- `iw`
- `iptables`
- `dnsmasq`
- `wpa_supplicant`

## 💻 Usage

  ./wlan78-ap

- You will be prompted to enter a password.
- Your access point will be created and start broadcasting.
- Connect with your smartphone, tablet or other Wi-Fi device.
- To check if your Wi-Fi interface supports AP mode, run the following command: **iw list | grep -A 10 "Supported interface modes**. You       should see the word 'AP' appear.

## Very Important

- Your access point 'wlan78' may refuse to reconnect after a password change. Consider **forgetting** this network on your smartphone or tablet, for example, then reconnect using the new password.

## To reset the access point setup and start over:

  ./wlan78-ap reset

## 🙋 Contact & Support

If you'd like to contact me, donate, or offer job opportunities in the Linux field, feel free to reach out:

📱 WhatsApp: **+216 55 504 712**

---
Made with ❤️ for the Linux community.
