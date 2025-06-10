# 🕵️ Flask Header Exploit & Defense Playground

## 🎯 Purpose
A hands-on lab environment to simulate and defend against header-based attacks:
- Host header injection
- CSP bypass
- X-Forwarded-For spoofing
- Origin and Referer misconfigurations

## 🔨 Tech Stack
- Flask
- Nginx reverse proxy (to observe header propagation)
- CSP, HSTS, and XSS lab setups for testing

## 🔐 Security Value
- **OWASP A03**: Injection
- **OWASP A05**: Security Misconfigurations
- Helps illustrate:
  - Why malformed or spoofed headers are dangerous
  - How to use headers for app hardening
  - Proxy configuration best practices

## 🧠 Features
- Web form to send custom headers (Host, Referer, XFF, etc.)
- Real-time output showing header impact
- Toggle defenses like:
  - CSP on/off
  - HSTS on/off
  - Origin validation
- Run behind Nginx to test real-world header behavior
- Docker support

## 🚀 Getting Started
```bash
# Clone repo
$ git clone https://github.com/yourusername/flask-header-playground.git
$ cd flask-header-playground

# Run using Docker
$ docker-compose up --build

# Or run locally
$ python3 -m venv venv && source venv/bin/activate
$ pip install -r requirements.txt
$ python run.py
```

## ✅ To Do
- [ ] Add report log for malformed headers
- [ ] Add more toggleable headers (Referrer-Policy, Permissions-Policy)
- [ ] Visual cue for whether a defense is active or not
- [ ] Curl command generator for common attacks

## 📄 License
MIT
