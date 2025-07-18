# AdminFinder

A fast, multi-threaded Python tool for discovering admin panels and login pages on web applications. AdminFinder uses a comprehensive wordlist of common admin paths to identify potential administrative interfaces.

## 🚀 Features

- **Multi-threaded scanning** - Configurable number of worker threads for fast scanning
- **Comprehensive wordlist** - Over 290 common admin panel paths and variations
- **Multiple file extensions** - Supports PHP, ASP, ASPX, HTML, CFM, JS, CGI, and BRF files
- **Colorized output** - Easy-to-read results with color-coded status messages
- **HTTP/HTTPS support** - Automatically handles both protocols
- **Error handling** - Graceful handling of network errors and timeouts

## 📋 Requirements

- Python 3.6+
- httpx
- colorama

## 🛠️ Installation

### Option 1: Clone from GitHub

```bash
# Clone the repository
git clone https://github.com/Mr3rf1/AdminFinder.git
cd AdminFinder

# Install dependencies
pip install -r requirments.txt

# Run the tool
python3 AdminFinder.py
```

### Option 2: Manual Installation

```bash
# Install Python dependencies
pip install httpx colorama

# Download the script
wget https://raw.githubusercontent.com/Mr3rf1/AdminFinder/main/AdminFinder.py

# Run the tool
python3 AdminFinder.py
```

## 🎯 Usage

1. **Run the script:**
   ```bash
   python3 AdminFinder.py
   ```

2. **Enter target URL:**
   - You can enter with or without protocol (http/https will be added automatically)
   - Examples: `example.com`, `https://target-site.com`, `192.168.1.100`

3. **Set number of workers:**
   - Recommended: 50-300 threads depending on your connection and target server
   - Higher values = faster scanning but more aggressive

### Example Session

```
    _       _           _       _____ _           _
   / \   __| |_ __ ___ (_)_ __ |  ___(_)_ __   __| | ___ _ __
  / _ \ / _` | '_ ` _ \| | '_ \| |_  | | '_ \ / _` |/ _ \ '__|
 / ___ \ (_| | | | | | | | | | |  _| | | | | | (_| |  __/ |
/_/   \_\__,_|_| |_| |_|_|_| |_|_|   |_|_| |_|\__,_|\___|_|

       github.com/Mr3rf1          t.me/Mr3rf1

 [<] Enter Url~> example.com
 [<] Enter Workers~> 100

 [*] Panel found ~> http://example.com/admin/
 [*] Panel found ~> http://example.com/login.php
 [!] Panel not found ~> http://example.com/administrator/
 ...

 [*] Panel Found: (in 15 seconds)
        http://example.com/admin/
        http://example.com/login.php
```

## 🔍 What It Scans

AdminFinder checks for common admin panel paths including:

- **Standard admin paths:** `/admin/`, `/administrator/`, `/adminpanel/`
- **Login pages:** `/login.php`, `/admin-login.html`, `/wp-login.php`
- **Control panels:** `/cpanel/`, `/controlpanel/`, `/admincp/`
- **CMS-specific paths:** WordPress, Joomla, Drupal admin areas
- **Various file extensions:** `.php`, `.asp`, `.aspx`, `.html`, `.cfm`, `.js`, `.cgi`

## ⚠️ Legal Disclaimer

**This tool is for educational and authorized security testing purposes only.**

- Only use this tool on websites you own or have explicit permission to test
- Unauthorized scanning of websites may violate laws and terms of service
- The authors are not responsible for any misuse of this tool
- Always ensure you have proper authorization before conducting security assessments

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## 📞 Contact

- **GitHub:** [Mr3rf1](https://github.com/Mr3rf1)
- **Telegram:** [@Mr3rf1](https://t.me/Mr3rf1)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**⭐ If you found this tool helpful, please give it a star!**
