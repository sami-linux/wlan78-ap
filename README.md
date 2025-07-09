# Linux Wi-Fi Access Point: wlan78-ap

## 📌 Why this script?

- 🪟 **Windows provides a built-in graphical tool** to create a Wi-Fi hotspot — but Linux does not.
- 🛠️ Tools like **hostapd** are **complex to configure** and are becoming **obsolete**.
- 🚀 This project offers a **simple way** to create a functional access point from any Linux system **without complex config files**.
- 🌐 This script is especially designed for people who don't have Ethernet access and want to use their Linux system as a Wi-Fi repeater of their existing Wi-Fi network.
- ✅ No need to touch any config file — everything is generated dynamically.

## ✅ Features

- Automatically detects a Wi-Fi interface connected to the Internet.
- Dynamically generates all necessary configuration files.
- Creates a virtual access point (`wlan78`) in seconds.
- Just type a password, and the AP is ready.
- Run `wlan78-ap reset` anytime to **reset and start clean**.

## 🧱 Requirements

Make sure your Wi-Fi interface supports AP mode (Access Point). It must be capable of acting as both a client (to get Internet) and a server (to share it) simultaneously.

Make sure the following tools are installed:

- `iw`
- `iptables`
- `dnsmasq`
- `wpa_supplicant`

## 💻 Usage

```bash
chmod +x wlan78-ap
sudo ./wlan78-ap
```

- You will be prompted to enter a password.
- Your access point will be created and start broadcasting.
- Connect with your smartphone, tablet or other Wi-Fi device.

To reset the access point setup and start over:

```bash
sudo ./wlan78-ap reset
```

## 🙋 Contact & Support

If you'd like to contact me, donate, or offer job opportunities in the Linux field, feel free to reach out:

📱 WhatsApp: **+216 55 504 712**

---
Made with ❤️ for the Linux community.
