# Firewall Configuration

## Allow SSH
```bash
sudo ufw allow ssh
```

## Set the Default Deny Policy
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

## Allow Port 8080
```bash
sudo ufw allow 8080/tcp
```

## What If SSH Was Not Allowed First?
If I ran `sudo ufw enable` before `sudo ufw allow ssh`, the default deny rule
would block port 22 and I would be locked out of my own server.
