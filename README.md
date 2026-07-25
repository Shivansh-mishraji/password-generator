# Multipurpose Security WebStack 🔐

<div align="center">

![Security WebStack Banner](https://capsule-render.vercel.app/api?type=venom&height=280&text=Security%20WebStack&fontSize=62&fontAlign=50&fontAlignY=52&color=0:0b132b,50:1c2541,100:0d3b3b&fontColor=5bc0be&desc=Password%20Forge%20%7C%20Hash%20Lab%20%7C%20Passphrase%20Studio%20%7C%20Session%20Vault&descFontColor=7dd3fc&descAlignY=72&animation=fadeIn)


<p>
  <img src="https://img.shields.io/badge/Python-3.12+-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Flask-3.x-000000?style=for-the-badge&logo=flask&logoColor=white" />
  <img src="https://img.shields.io/badge/Vercel-Deployed-000000?style=for-the-badge&logo=vercel&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Live-1f9d55?style=for-the-badge" />
</p>

**A full-stack Flask web app for secure password generation, passphrase creation, cryptographic hashing, and live strength analysis.**

[![Live Demo](https://img.shields.io/badge/🌐_Live_Demo-Try_It_Now-7C3AED?style=for-the-badge)](https://random-password-generator-by-shivansh-mishra.vercel.app/)

</div>

---

## 🎯 What Is This?

Security WebStack is a **production-deployed security toolkit** built with Python + Flask, providing day-to-day cryptographic utilities through a clean, intuitive web interface. No heavy frameworks, no unnecessary complexity — just practical, reliable security tools.

**Built as a team project** led by Shivansh Mishra, designed for real-world use and deployed on Vercel.

---

## ✨ Features

| Module | Description |
|---|---|
| 🔐 **Password Forge** | Configurable password generation with live strength score & telemetry charts |
| 🧠 **Passphrase Studio** | Generate memorable high-entropy passphrases (BIP-39 style) |
| 🧪 **Hash Lab** | Generate and verify cryptographic digests (MD5, SHA-1, SHA-256, SHA-512) |
| 🗂️ **Session Vault** | Save, manage, import & export passwords as JSON — browser-local only |
| 📊 **Strength Telemetry** | Real-time visual feedback on password entropy and weakness patterns |
| ⚡ **Batch Mode** | Generate multiple passwords at once for bulk use cases |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python 3.12 + Flask 3.x |
| Crypto | `secrets` (randomness) + `hashlib` (hashing) |
| Frontend | Vanilla JS + CSS (no heavy frameworks) |
| Deployment | Vercel (serverless via `vercel.json`) |
| WSGI | `wsgi.py` for production server |

---

## 🔒 Security Design

- **True Randomness**: Password generation uses Python's `secrets` module (CSPRNG), not `random`
- **Client-Side Vault**: All saved passwords stay in your browser (`sessionStorage`) — never sent to any server
- **No Data Logging**: Zero server-side storage of passwords, passphrases, or hashes
- **Open Source**: Full transparency — read the code yourself

---

## 🗂️ Project Structure

```
password-generator/
├── Random_Password_Generator.py  # Core Flask app + all routes
├── api/                          # Vercel serverless API handler
├── static/                       # CSS, JS, assets
├── templates/                    # Jinja2 HTML templates
├── wsgi.py                       # WSGI entrypoint for production
├── requirements.txt              # Python dependencies
├── vercel.json                   # Vercel deployment config
└── Procfile                      # Heroku/Render entrypoint
```

---

## 🚀 Run Locally

```bash
# 1. Clone the repo
git clone https://github.com/Shivanshmishra7275/Random-Password-Generator.git
cd Random-Password-Generator

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the app
python Random_Password_Generator.py
```

Open **http://127.0.0.1:5000** in your browser.

---

## 🌐 API Endpoints

| Endpoint | Method | Description |
|---|---|---|
| `/` | GET | Main app UI |
| `/healthz` | GET | Health check → `{"status":"ok"}` |
| `/generate` | POST | Generate password(s) |
| `/hash` | POST | Hash a string |
| `/verify` | POST | Verify hash match |

---

## 👥 Team

| Role | Name |
|---|---|
| 🏆 Leader | Shivansh Mishra |
| 👨‍💻 Member | Ravi Gupta |
| 👨‍💻 Member | Harshvardhan Sisodiya |
| 👨‍💻 Member | Vishal Patel |
| 👨‍💻 Member | Dhuru Madhuwal |

---

## 👤 Lead Developer

**Shivansh Mishra** — ML Builder & AI Product Explorer
📍 Lucknow, India · [GitHub](https://github.com/Shivansh-mishraji) · [Portfolio](https://shivansh-mishraji.github.io/Portfolio-Website/)

---

<div align="center">
  <i>Built for real-world use · Deployed on Vercel · Zero server-side data storage</i>
</div>
