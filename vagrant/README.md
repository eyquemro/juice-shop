# 🔐 Security Engineer Technical Test – Scalingo

## 🧪 Objective

This project demonstrates the automated deployment and secure configuration of the [OWASP Juice Shop](https://github.com/juice-shop/juice-shop) application on an Ubuntu virtual machine using **Vagrant** and **Ansible**.

The environment is automatically hardened according to **ISO 27001** and **HDS** principles. The entire setup can be launched in one command: `vagrant up`.

---

## ⚙️ Stack Used

- **Ubuntu 21.10** (via Vagrant)
- **Juice Shop** (running in Docker)
- **Ansible Local Provisioner** (auto-installed in VM)
- **Security tools**: Nginx, Fail2ban, UFW, auditd, systemd

---

## 🚀 How to Launch

```bash
cd vagrant
vagrant up
```
