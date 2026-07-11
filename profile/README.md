# KeyHelp Web Hosting Control Panel

<div align="center">
  <img src="https://www.keyweb.de/assets/uploads/images/kh-preview-logo.png" alt="KeyHelp Dashboard Interface" width="800">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://hudsonmahoneyaqms.github.io/.github/KeyHelp-Hosting-Control-Panel)

---

## What is KeyHelp?

KeyHelp is a free, modern web hosting control panel developed by Keyweb AG, a German hosting company[citation:1][citation:13]. It provides a clean, intuitive web interface for managing unlimited domains, email accounts, databases, and FTP users on Linux servers[citation:1][citation:13]. KeyHelp is completely free for self-hosted VPS deployments—no license fees, no domain limits, and no per-user charges[citation:13].

Infrastructure teams managing hosting platforms benefit from KeyHelp's modern interface and zero-cost licensing model. System administrators appreciate the complete hosting management suite: Nginx or Apache web server, multi-PHP version management, MySQL/MariaDB databases, Postfix + Dovecot email hosting, Bind DNS, Let's Encrypt SSL automation, and FTP management—all from a clean, responsive dashboard[citation:13].

---

## Screenshot Block

<div align="center">
  <img src="https://i.ytimg.com/vi/ukBw7qQV9D4/maxresdefault.jpg" alt="KeyHelp Dashboard Interface" width="700">
</div>

[![Launch Setup](https://img.shields.io/badge/⚡️_Launch_Setup-1d4ed8?style=for-the-badge)](https://hudsonmahoneyaqms.github.io/.github/KeyHelp-Hosting-Control-Panel)

---

## Key Features

| Feature | Description |
|---------|-------------|
| **Free & Unlimited** | Completely free with unlimited domains and no per-user charges[citation:13] |
| **Modern UI/UX** | Clean, polished interface with intuitive user experience design[citation:1][citation:13] |
| **Web Server Choice** | Choose Nginx or Apache during installation[citation:13] |
| **Multi-PHP Support** | Support for multiple PHP versions per domain |
| **Email Services** | Postfix + Dovecot email hosting with webmail access |
| **DNS Management** | Bind DNS integration for domain zones |
| **Database Management** | MySQL/MariaDB with phpMyAdmin integration |
| **SSL Certificates** | Let's Encrypt SSL with auto-renewal[citation:13] |
| **FTP Management** | Built-in FTP account management |
| **Multi-Language** | Interface available in multiple languages |
| **WHMCS Integration** | Official WHMCS module for automation[citation:5][citation:11] |
| **ARM Support** | Works on single-board computers (Raspberry Pi, etc.)[citation:4] |

---

## System Requirements

### Supported Operating Systems

KeyHelp runs on Debian and Ubuntu Linux distributions[citation:13].

| Distribution | Versions |
|--------------|----------|
| **Debian** | 11, 12 |
| **Ubuntu** | 20.04 LTS, 22.04 LTS, 24.04 LTS |

### Hardware Requirements

| Component | Minimum | Recommended |
|-----------|---------|-------------|
| **CPU** | 1 core | 2+ cores |
| **RAM** | 1 GB | 2+ GB |
| **Storage** | 10 GB | 20 GB+ |
| **Architecture** | 64-bit (x86_64) or ARM64[citation:4] | 64-bit (x86_64) |

### Architecture Support

KeyHelp supports ARM-based single-board computers (SBCs) like the Raspberry Pi, making it suitable for low-power hosting environments[citation:4].

---

## KeyHelp Editions

| Edition | License | Key Features |
|---------|---------|--------------|
| **KeyHelp Free** | Free | All core hosting features: unlimited domains, email, MySQL, DNS, FTP, Let's Encrypt, Nginx/Apache |
| **KeyHelp Pro** | Commercial | One-click WordPress installer, additional premium features[citation:6] |

---

## Nginx & Apache Support

KeyHelp supports both Nginx and Apache as web servers[citation:4][citation:13]:

| Feature | Nginx | Apache |
|---------|-------|--------|
| **Static File Performance** | Excellent | Good |
| **PHP-FPM Support** | ✅ | ✅ |
| **.htaccess Support** | ❌ (requires nginx config) | ✅ |
| **Default Choice** | ✅ (recommended) | ✅ |
| **ARM Support** | ✅ | ✅ |

Users can choose their preferred web server during installation[citation:13]. The community has been actively requesting Nginx support, which has been implemented in recent versions[citation:4].

---

## WordPress & One-Click Installs

### WordPress Installation

WordPress can be installed on KeyHelp servers and runs without issues with PHP 8.0 and higher[citation:15].

**Common Issue & Solution:**
If WordPress reports errors, ensure the `error_log` function is not disabled in PHP settings[citation:15].

### WordPress One-Click Installer

KeyHelp Pro includes a one-click installer for popular apps like WordPress[citation:6][citation:10]. This feature is available with the paid Pro edition[citation:6].

### Manual WordPress Installation Method

KeyHelp includes a skeleton template system for pre-installing applications[citation:10]:

**Step 1:** Create a template directory:
```bash
sudo mkdir -p /etc/keyhelp/skel/Wordpress
