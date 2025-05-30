# Hardening Measures (ISO 27001 / HDS Mapping)

| # | Security Measure           | Description                                                | ISO 27001 / HDS |
|---|----------------------------|------------------------------------------------------------|-----------------|
| 1 | Non-root user              | Juice Shop runs as a dedicated, non-privileged user        | A.9.2.3         |
| 2 | UFW Firewall               | Only ports 22, 80, 443 are allowed                         | A.13.1.1        |
| 3 | Fail2ban                   | Protects SSH from brute-force attacks                      | A.12.4.1        |
| 4 | HTTPS (self-signed TLS)   | Juice Shop exposed via secure Nginx reverse proxy          | A.13.2.3        |
| 5 | System log hardening       | Logs are collected and protected via auditd                | A.12.4.3        |
| 6 | File permission hardening | Juice Shop directory has restricted access (chmod 750)     | A.9.4.1         |
| 7 | SSH root login disabled    | Access restricted to the vagrant user                      | A.9.2.4         |
| 8 | Auto-start with systemd    | Juice Shop runs persistently at boot                       | A.12.4.1        |
| 9 | Removal of unused packages | Reduces attack surface                                     | A.13.1.2        |
| 10| Nginx reverse proxy        | Isolates Juice Shop and enables TLS termination            | A.13.1.3        |
