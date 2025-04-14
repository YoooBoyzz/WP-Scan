
# WP-Scan 🔍🔐

WP-Scan is a CLI-based WordPress vulnerability scanner designed for security professionals and website owners to audit their WordPress site's security. ⚔️🛡️

**✨ Features**:

- 🔍 Detect WordPress version and known vulnerabilities.
- 🧩 Identify installed plugins & themes and their vulnerabilities.
- 👥 Enumerate WordPress users.
- 🧠 Brute-force user passwords.
- ⚙️ Detect exposed configuration or database files.
- ⚠️ Detect exposed plugin log files.
- 🖼️ Enumerate media files & uploads directory.
- 🐛 Identify vulnerable Timthumb files.
- 📘 Check for existence of readme file.
- ⏰ Check if WP-Cron and user registration are enabled.
- 🧵 Detect Full Path Disclosure.


# ⚙️ Installation


## 📱 Running WP-Scan on Termux (Android)

1. **🛠️ Update & Install Dependencies**
```bash
pkg update && pkg upgrade
pkg install python git
```

2. **🔽 Clone WP-Scan Repository**
```bash
git clone https://github.com/YoooBoyzz/WP-Scan.git
cd WP-Scan
```

3. **📦 Install Requirements**
```bash
pip install requests bs4
```


## 🖥 Running With Linux (Ubuntu/Debian)

1. **⚒️ install dependencies**
```bash
 sudo apt update && sudo apt install python3 python3-pip git
```

2. **🔽 Clone WP-Scan Repository**
```bash
git clone https://github.com/YoooBoyzz/WP-Scan.git
cd WP-Scan
```

3. **📦 Install Requirements**
```bash
pip3 install requests bs4
```


### **▶️ Run WP-Scan**:

```bash
python3 wpbrute.py
```


### License

This project is open source and available under the [MIT License](LICENSE).
