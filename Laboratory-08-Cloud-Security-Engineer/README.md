# Laboratory Activity 8 – Mission 8: The Cloud Security Engineer

## Mission Overview
In this lab, I secured a new Ubuntu server that was left exposed to the
internet. I deployed an Nginx web app in a container, then used UFW to allow
SSH, block all other incoming traffic by default, and open only port 8080 for
the web app.

## Objectives
- Understand the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure UFW with a Default Deny policy.
- Allow SSH and HTTP traffic using specific port rules.
- Document firewall rules and security best practices in Markdown.
- Continue expanding my GitHub Cloud Computing Portfolio.

## Commands Executed
| Command | Purpose |
|---|---|
| `docker run -d -p 8080:80 --name secure-web-app nginx` | Deploy the Nginx web app on port 8080 |
| `curl http://localhost:8080` | Check that the app responds |
| `sudo ufw allow ssh` | Allow SSH (port 22) before enabling the firewall |
| `sudo ufw default deny incoming` | Block all incoming traffic by default |
| `sudo ufw default allow outgoing` | Allow all outgoing traffic |
| `sudo ufw enable` | Turn on the firewall |
| `sudo ufw status verbose` | Check the firewall status and default policies |
| `sudo ufw allow 8080/tcp` | Allow TCP traffic on port 8080 |
| `sudo ufw status numbered` | List the firewall rules with numbers |

## Skills Learned
I learned how to set up UFW from the command line, apply Default Deny, and
open only the ports a service needs. I also learned why SSH has to be allowed
before enabling a firewall, and how to document security settings clearly.
