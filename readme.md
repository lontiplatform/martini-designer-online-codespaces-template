# Martini Designer Online – GitHub Codespaces Setup

This repository provides a ready-to-use **GitHub Codespaces** environment for running **Martini Designer Online** entirely in the cloud — no local installation required.

Martini Designer Online enables fast, browser-based development within a fully configured container environment.

---

## Quick Start

1. **Clone this repository**  
   Click the **Code** button on this repository and select **Open with Codespaces**,  
   or clone it to your own GitHub account.

2. **Open in Codespaces**  
   Launch a new Codespace for this repository.  
   GitHub will automatically initialize the environment using the included `.devcontainer` configuration.

3. **Set required Codespaces secrets**  
   Before starting Martini Designer Online, make sure you define the following **Codespaces Secrets** under your GitHub account or organization:

   | Secret Name | Description |
   |--------------|-------------|
   | `MARTINI_LICENSE` | Your valid Martini Designer license key (required for activation). |
   | `MARTINI_IMAGE_TAG` | *(Optional)* Martini Designer image tag to use (e.g. `latest`, `1.0.5`). Defaults to `latest`. |

   **To add them:**  
   - Go to your repository → **Settings → Secrets and variables → Codespaces → New secret**  
   - Enter each name and its value, then save.  
   - Codespaces will inject them automatically into the container environment.

4. **Wait for setup**  
   Codespaces builds the environment, pulls the Martini Designer Docker image, and starts the container using Docker Compose.

5. **Access Martini Designer Online**  
   Once setup completes, open the **Ports** tab and locate **port 3000**.  
   Click **Open in Browser** to launch the Martini Designer Online interface.

---

## Configuration Overview

| File | Purpose |
|------|----------|
| `.devcontainer/devcontainer.json` | Defines the Codespaces configuration, ports, and environment variables. |
| `.devcontainer/docker-compose.yml` | Runs the Martini Designer container and mounts the workspace volume. |
| `workspace/` | Optional folder for storing your Martini projects persistently. |

---

## Notes & Best Practices

- **Machine size:** Adjust Codespace resources (CPU/RAM) based on your workload.  
- **Idle timeout:** Codespaces stop automatically when inactive — save your work often.  
- **Cost control:** Shut down unused Codespaces to manage compute usage.  
- **Network stability:** A reliable connection improves performance and build times.

---

## Additional Resources

- [Martini Designer Online – GitHub Codespaces Installation Guide](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/installation/github-codespaces/#notes)
- [Martini Designer Online Self-Managed Hosting](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/) *(check for updates and advanced configuration)*
- [Lonti Official GitHub Organization](https://github.com/lontiplatform)

---

**Maintained by Lonti Platform**  
For updates or issues, check the [official documentation](https://developer.lonti.com/).
