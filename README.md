
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
🐧 Linux (Debian/Ubuntu)

```bash
sudo apt update && sudo apt install ruby-full git build-essential libcurl4-openssl-dev libssl-dev zlib1g-dev -y
sudo gem install wpscan
```

### 🐳 Docker

```bash
docker pull wpscanteam/wpscan
```

### 🍎 Homebrew (macOS)

```bash
brew install wpscanteam/tap/wpscan
```

### ▶️ Basic Usage

Scan a site:

```bash
wpscan --url https://example.com
```

Enumerate users:

```bash
wpscan --url https://example.com --enumerate u
```

Stealth mode (silent scan):

```bash
wpscan --stealthy --url https://example.com
```

Show all options:

```bash
wpscan --help
```

# 🔄 Updates
Update vulnerability database:

```bash
wpscan --update
```

Update WPScan itself:

```bash
gem update wpscan
```


## 📱 Running WP-Scan on Termux (Android)

1. **🛠️ Update & Install Dependencies**
```bash
pkg update && pkg upgrade
pkg install git ruby -y
gem install bundler
```

2. **🔽 Clone WP-Scan Repository**
```bash
git clone https://github.com/YoooBoyzz/WP-Scan.git
cd WP-Scan
```

3. **📦 Install Ruby Dependencies**
```bash
bundle install
```


If bundle install throws errors, try:

```bash
gem install nokogiri
gem install public_suffix
```

4. **▶️ Run WP-Scan**:
```bash
ruby wpscan.rb --url https://example.com
```
Or:

```bash
ruby bin/wpscan --url https://example.com
```


### License

This project is open source and available under the [MIT License](LICENSE).
