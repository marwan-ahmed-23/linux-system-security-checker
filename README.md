# 🛡️ Linux System Security Checker

A lightweight and powerful **Bash script** designed to perform a quick security audit of your Linux system. This tool checks for firewall status, sensitive file permissions, inactive users, and running services, then generates a detailed security report.

---

## 🚀 Features
- 🔥 **Firewall Status**: Checks if UFW is active and lists current rules.
- 🔐 **Sensitive File Permissions**: Verifies permissions for critical files like `/etc/passwd` and `/etc/shadow`.
- 👤 **Inactive User Accounts**: Detects unused or suspicious accounts.
- 🛠️ **Service Monitoring**: Lists top 10 running services based on memory usage.
- 📝 **Detailed Report**: Automatically generates a comprehensive security report.


## 📂 Directory Structure
```plaintext
linux-system-security-checker/
├── security-checker.sh   # The main Bash script
├── README.md             # Documentation
├── LICENSE
└── example-report.txt    # Example output of the security report
```

## 📖 Usage
1. Clone this repository:

    ```bash
    git clone https://github.com/marwan-ahmed-23/linux-system-security-checker.git
    cd linux-system-security-checker
    ```

2. Make the script executable:

    ```bash
    chmod +x security-checker.sh
    ```

3. Run the script:

    ```bash
    ./security-checker.sh
    ```
    
4. View the generated report:

    ```bash
    cat security-report.txt
    ```

## 🖼️ Example Report

Here's an example of the output generated by the script:

```plaintext
Security Report - Thu Dec 21 2024
---------------------------------------
Firewall Status:
Status: active

To                         Action      From
--                         ------      ----
22                         ALLOW       Anywhere
---------------------------------------
File Permissions:
/etc/passwd -rw-r--r--
/etc/shadow -rw-------
/etc/hosts -rw-r--r--
---------------------------------------
Inactive Users:
root
admin
---------------------------------------
Top 10 Running Services by Memory Usage:
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root         1  0.0  0.1 102400  9280 ?       Ss   12:00   0:03 /sbin/init
mysql      172  0.5  1.5 125000 11000 ?       Ssl  12:00   0:30 /usr/sbin/mysqld
```

## 🛠️ Contributing

We welcome contributions to improve this tool! Here's how you can help:

- 🐛 **Report issues:** Found a bug? Open an issue and let us know.
- 🌟 **Suggest features:** Have an idea for improvement? We'd love to hear it.
- 🔧 **Submit pull requests:** Contribute code directly to the repository.

## 🌟 Show Your Support
If you found this project helpful, please consider giving it a ⭐ on GitHub. Your support means the world to us!






