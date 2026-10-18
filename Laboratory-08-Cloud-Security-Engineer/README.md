# Mission 8: The Cloud Security Engineer

## Mission Overview
This activity secures a newly deployed Ubuntu server that was left exposed to
the public internet. Acting as a Cloud Security Engineer, I deployed an Nginx
web application, then locked the server down with the Uncomplicated Firewall
(UFW): allowing SSH first, enforcing a Default Deny policy for incoming
traffic, and opening only port 8080 for the web application.

## Objectives
- Understand the concept of the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure the Uncomplicated Firewall (UFW) with a Default Deny policy.
- Implement granular port management to selectively allow SSH and HTTP traffic.
- Document firewall rules and security best practices using Markdown.
- Continue expanding my professional GitHub Cloud Computing Portfolio.

## Commands Executed
| Command | Purpose |
|---|---|
| `docker run -d -p 8080:80 --name secure-web-app nginx` | Deploy the Nginx web application on port 8080 |
| `curl http://localhost:8080` | Verify the application is reachable |
| `sudo ufw allow ssh` | Permanently allow SSH (port 22) before enabling the firewall |
| `sudo ufw default deny incoming` | Block all incoming traffic by default |
| `sudo ufw default allow outgoing` | Allow all outgoing traffic |
| `sudo ufw enable` | Activate the firewall |
| `sudo ufw status verbose` | Check the firewall status and default policies |
| `sudo ufw allow 8080/tcp` | Explicitly allow TCP traffic on port 8080 |
| `sudo ufw status numbered` | List the firewall rules with numbers |

## Skills Learned
Applying the Principle of Least Privilege and Default Deny in practice;
configuring UFW from the command line; allowing specific services by port
while blocking everything else; understanding why SSH must be allowed before
enabling a firewall; and documenting security configurations clearly in
Markdown.
