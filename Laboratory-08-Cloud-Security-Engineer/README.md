# Laboratory Activity 8: Mission 8 – The Cloud Security Engineer

## Mission Overview
This laboratory focuses on applying defense-in-depth principles by securing an active server using a host-based firewall. The activity involves setting up a publicly accessible web application, checking open network ports, and configuring UFW with a Default Deny policy to restrict incoming connections to only the services required by the application.

## Objectives
- Learn about the server's attack surface and the Principle of Least Privilege
- Conduct a basic inspection of currently active network ports
- Set up UFW using a Default Deny configuration
- Manage network access by allowing only necessary SSH and web application traffic

## Commands Executed
- `docker run -d --name secure-web-app -p 8080:80 nginx` — launched an Nginx web application accessible through port 8080
- `sudo ufw allow ssh` — created an SSH access rule before activating the firewall
- `sudo ufw default deny incoming` / `sudo ufw default allow outgoing` — configured the firewall to block incoming connections while permitting outgoing traffic
- `sudo ufw enable` — turned on the firewall
- `sudo ufw status verbose` — checked the firewall's current state and configuration
- `sudo ufw allow 8080/tcp` — permitted incoming connections through the web application's port
- `sudo ufw status numbered` — reviewed the numbered list of active firewall rules

## Skills Learned
- Setting up and managing UFW as a server-side firewall
- Applying a Default Deny policy to improve server security
- Recognizing the importance of allowing SSH access before enabling the firewall
- Controlling network ports to reduce unnecessary exposure
- Properly recording firewall settings and security configurations for future reference
