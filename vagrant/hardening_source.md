## 🔐 Hardening Measures — ISO/IEC 27001:2013 Mapping

These security hardening measures follow the [OWASP Juice Shop Hardening Guide](https://pwning.owasp-juice.shop/part2/hardening.html) and are aligned with ISO/IEC 27001:2013 controls.

| #  | Security Measure               | Description                                                              | ISO/IEC 27001:2013 Control                                 | Reference / Source                                                                 |
|----|-------------------------------|--------------------------------------------------------------------------|------------------------------------------------------------|------------------------------------------------------------------------------------|
| 1  | UFW Firewall                   | Only ports 22 (SSH), 80 (HTTP), 443 (HTTPS) are allowed                  | A.13.1.1 – Network controls                                 | [A.13.1.1 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1311)    |
| 2  | Fail2ban                       | Detects and blocks brute-force attacks by monitoring SSH logs           | A.12.6.1 – Technical vulnerability management               | [A.12.6.1 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1261)    |
| 3  | HTTPS (TLS Certificate)        | Encrypted traffic via Nginx reverse proxy using TLS (SSL)               | A.13.2.3 – Protection of information in transit             | [A.13.2.3 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1323)    |
| 4  | System Logging (auditd)        | Logs system events and protects log integrity                           | A.12.4.1 – Event logging                                     | [A.12.4.1 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1241)    |
| 5  | SSH Root Login Disabled        | SSH access restricted to non-root users                                 | A.9.2.4 – Management of secret authentication information   | [A.9.2.4 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a924)      |
| 6  | Removal of Unused Packages     | Reduces system attack surface                                           | A.12.1.2 – Change management                                | [A.12.1.2 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1212)    |
| 7  | Nginx Reverse Proxy Isolation  | Isolates Juice Shop and handles secure TLS termination                  | A.13.1.3 – Segregation in networks                          | [A.13.1.3 – iso-docs.com](https://iso-docs.com/blogs/iso-27001-standard#a1313)    |
