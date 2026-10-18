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
If `sudo ufw enable` were run before `sudo ufw allow ssh`, the Default Deny
policy would block port 22 and lock the administrator out of the server's
remote access.
