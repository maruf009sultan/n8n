# 🚀 One-Click Deployable n8n on Docker – Automate Everything with Style!

![Banner](https://cdn.pixabay.com/photo/2017/05/15/23/47/machine-learning-2749148_1280.jpg)
[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/maruf009sultan/n8n)
> 🔧 Powerful. Fast. Beautiful.  
> **Deploy n8n in seconds with Docker — no setup required.**

---

## 💡 What is This?

This repository contains a **Dockerized version of [n8n](https://n8n.io)** — the open-source, extendable workflow automation tool that lets you connect everything and automate anything.  
With n8n you can create powerful workflows visually, automate repetitive tasks, integrate with 1000+ apps/services, and unleash creativity without writing code (unless you want to!).

---

## 🌟 Why This Docker Image?

- **🚀 1-Click Deploy** – Instantly launch n8n with zero config!
- **🎨 Gorgeous, Modern UI** – Drag, drop, automate, and visualize your logic.
- **⚡ Lightning Fast** – Ready-to-go, optimized, and cloud-friendly.
- **🔒 Secure & Minimal** – Clean Node 18 base, minimal attack surface.
- **🌎 Cloud Ready** – Works on Render, Railway, Heroku, AWS, DigitalOcean, or your own server.
- **🕹️ Flexible** – Tweak with simple environment vars. BYO database, domain, SSL, etc.

---

## 🌐 Live Demo

Experience n8n instantly:  
[https://n8n-dhrr.onrender.com](https://n8n-dhrr.onrender.com)

> _This is a public demo. For production, self-host your own instance below!_

---

## ☁️ One-Click Deploy to the Cloud

| Platform | Deploy |
|----------|--------|
| **Render**  | [![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/maruf009sultan/n8n) |
| **Heroku**  | [![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/maruf009sultan/n8n) |
| **Railway** | [![Deploy on Railway](https://railway.com/button.svg)](https://railway.com/deploy/7IisQg?referralCode=fbROj8) |

> 💡 Just click, authorize, and your own n8n instance will be live in minutes!

---

## 🐳 Local Docker Setup

### 1. **Build the image**
```bash
docker build -t my-n8n .
```

### 2. **Run the container**
```bash
docker run -d -p 80:80 --name n8n-container my-n8n
```

- 🚀 Visit [http://localhost](http://localhost) in your browser to start automating!

> Need persistent data? Mount a volume for `/root/.n8n`!

---

## ⚙️ How Does It Work?

- **From Source:** Uses official `node:18` as the base.
- **Global Install:** Installs latest n8n (with npm) & Git (for pulling custom nodes).
- **Config:** Auto-sets port, protocol, and public URLs via environment variables.
- **Runs at Port 80:** No need to mess with ports — just access and go!

### Under the Hood:

1. 🛠️ Installs Git & n8n globally  
2. 📂 Creates required data folders  
3. 🌍 Exposes port 80  
4. 🏁 Starts n8n — ready for your workflows!

---

## ⚡ Environment Variables

Fine-tune your instance with these env vars (all optional!):

| Variable | Default | Description |
|----------|---------|-------------|
| `N8N_PORT` | `80` | Port to expose |
| `N8N_HOST` | `0.0.0.0` | Bind address |
| `N8N_PROTOCOL` | `http` | Use `https` for SSL |
| `N8N_EDITOR_BASE_URL` | `https://n8n-dhrr.onrender.com` | Public editor URL |
| `WEBHOOK_TUNNEL_URL` | `https://n8n-dhrr.onrender.com` | Public webhook endpoint |
| `N8N_DIAGNOSTICS_ENABLED` | `false` | Telemetry setting |
| `N8N_VERSION_NOTIFICATIONS_ENABLED` | `false` | Update checks |

Example advanced run:

```bash
docker run -d \
  -p 8080:80 \
  -e N8N_EDITOR_BASE_URL=https://my-n8n.example.com \
  -e WEBHOOK_TUNNEL_URL=https://my-n8n.example.com \
  --name my-n8n maruf009sultan/n8n
```

---

## 🌈 Why You'll Love n8n

- 🎛️ **Visual Workflow Designer** – Build automations with drag-and-drop simplicity.
- 🔗 **1000+ Integrations** – Connect to Slack, Discord, Gmail, databases, APIs, and more.
- 🏗️ **Custom Nodes** – Extend with your own code or community plugins.
- 🕰️ **Trigger Anything** – Schedules, webhooks, API calls, email, cron, and beyond.
- 🌍 **Self-Hosted Freedom** – Own your data, your way.
- 💾 **Persistent & Cloud-Native** – Works with Docker volumes, cloud storage, or your own DB.

---

## 🚀 Use Cases

- 📨 Auto-respond to emails or messages
- 🔄 Sync data between Google Sheets and databases
- 🤖 Build chatbots, notifications, or smart alerts
- 📊 Generate and send automated reports
- 🛠️ Orchestrate CI/CD, devops, and more

---

## 🏗️ Example Workflow

![n8n Workflow Example](https://raw.githubusercontent.com/n8n-io/n8n/master/assets/n8n-editor-example.png)

---

## 📚 Learn More

- [n8n Official Docs](https://docs.n8n.io)
- [Awesome n8n Workflows](https://n8n.io/workflows)
- [n8n Community Forum](https://community.n8n.io)

---

## ❤️ Like This Project?

Show some love:  
⭐ Star this repo  
🍴 Fork it  
🗣️ Share with friends  
🚀 Submit PRs or ideas!

---

## 💬 Questions? Feedback?

- Open an [issue](https://github.com/maruf009sultan/n8n/issues)
- Reach out on [n8n Community](https://community.n8n.io)
- Let’s make automation beautiful together! 🎨

---

> Created with ❤️ by [maruf009sultan](https://github.com/maruf009sultan)  
> MIT License – Free to use, modify, and share

---
