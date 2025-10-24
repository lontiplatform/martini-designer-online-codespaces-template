# Martini Designer Online – GitHub Codespaces Template

This repository provides a ready-to-use **GitHub Codespaces** setup for running **Martini Designer Online** in the cloud — no local installation required.

Martini Designer Online enables fast, browser-based development and deployment within a pre-configured Codespaces environment.

---

## 🚀 Quick Start

1. **Clone this repository**  
   Click the **Code** button on this repository and select **Open with Codespaces** or **Clone** it to your own GitHub account.

2. **Open in Codespaces**  
   After creating your repo, click **Code → Open with Codespaces** to launch a new development environment.

3. **Wait for setup**  
   GitHub Codespaces automatically builds the environment using the included `.devcontainer` configuration and Docker Compose file.  
   This process installs dependencies and prepares Martini Designer Online for use.

4. **Run Martini Designer Online**  
   Once the Codespace starts, open the **Ports** tab and locate port `3000`.  
   Click **Open in Browser** to access the Martini Designer Online interface.

---

## ⚙️ Configuration Overview

| File | Purpose |
|------|----------|
| `.devcontainer/devcontainer.json` | Defines the Codespaces environment and port configuration |
| `.devcontainer/docker-compose.yml` | Runs Martini Designer Online inside a Docker container |
| `workspace/` | Optional persistent workspace for saving projects |

---

## 🧠 Notes & Considerations

- **Machine size:** Choose a Codespaces machine size that fits your workload.
- **Session limits:** Idle Codespaces stop automatically after a timeout.
- **Network stability:** A consistent internet connection ensures smoother usage.
- **Cost control:** Shut down idle Codespaces to manage compute time efficiently.

---

## 📚 Additional Resources

- [GitHub Codespaces Quickstart Guide](https://docs.github.com/en/codespaces/getting-started/quickstart)
- [Martini Designer Online Self-Managed Hosting](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/) *(check for updates and advanced configuration)*

---

**Maintained by Lonti Platform.**  
For updates or issues, visit the [official Lonti GitHub organization](https://github.com/Lonti).
