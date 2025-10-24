# Martini Designer Online Codespaces Template

This repository provides the official **Codespaces template** for running Martini Designer Online in a preconfigured GitHub Codespaces environment.  

It allows developers to quickly launch Martini Designer Online entirely in the cloud, without requiring any local setup.  
All necessary container and environment configurations are included for immediate use.

## Quick Start

1. **Clone the repository**  
   Visit the [Martini Designer Online Codespaces Installation Guide](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/installation/github-codespaces/#notes)  
   and clone this repository.

2. **Push changes to your remote repository**  
   After cloning or forking, customize the configuration files in `.devcontainer` or other folders as needed.  
   Once your setup is ready, commit and push the changes to your own GitHub repository.

3. **Create a new Codespace (from the GitHub web interface)**  
   - Go to your repository page in GitHub.  
   - In the top-left corner of the GitHub interface, click the **menu icon** to expand the sidebar then click **Codespaces**.  
   - Click **New codespace**.  
   - Choose:
     - **Repository:** your forked or cloned repository  
     - **Branch:** select the branch you want to use  
     - **Region:** select the region closest to your users  
     - **Machine type:** choose CPU/RAM configuration as needed  
   - Click **Create codespace** to start the environment.

4. **Set required Codespaces secrets**  
   Before starting Martini Designer Online, define the following Codespaces secrets under your GitHub account or organization:

   | Secret Name | Description |
   |--------------|-------------|
   | `MARTINI_LICENSE` | Your valid Martini Designer license key (required for activation). |
   | `MARTINI_IMAGE_TAG` | Optional. Martini Designer image tag to use (for example, `latest`, `1.0.5`). Defaults to `latest`. |

   To add them:  
   - Go to your repository → **Settings → Secrets and variables → Codespaces → New secret**  
   - Enter each name and value, then save.  
   - Codespaces will automatically inject them into the container environment.

5. **Wait for setup**  
   Codespaces automatically builds the environment, pulls the Martini Designer Docker image, and starts the container using Docker Compose.

6. **Access Martini Designer Online**  
   Once setup completes, open the **Ports** tab and locate **port 3000**.  
   Click **Open in Browser** to launch the Martini Designer Online interface.

## Configuration Overview

| File | Purpose |
|------|----------|
| `.devcontainer/devcontainer.json` | Defines the Codespaces configuration, ports, and environment variables. |
| `.devcontainer/docker-compose.yml` | Runs the Martini Designer container and mounts the workspace volume. |
| `workspace/` | Workspace directory for storing Martini projects persistently. |

## Notes 

- **Machine size:** Adjust Codespace resources (CPU and RAM) based on your workload.  
- **Idle timeout:** Codespaces stop automatically when inactive, so save your work frequently.  

## Additional Resources

- [Martini Designer Online - GitHub Codespaces Installation Guide](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/installation/github-codespaces/#notes)
- [Martini Designer Online Self-Managed Hosting](https://developer.lonti.com/docs/martini/installation-configuration/designer-online/self-managed/) *(check for updates and advanced configuration)*

Maintained by Lonti Platform.  
For updates or issues, refer to the [official documentation](https://developer.lontiplatform.com/).
