# Firewall Configuration

## Allow SSH
```bash
sudo ufw allow ssh
```

This rule allows SSH connections so administrators can remotely manage the server.

## Default Firewall Policies
```bash
sudo ufw default deny incoming
sudo ufw default allow outgoing
```

These rules block incoming connections by default while allowing outgoing connections.

## Enable UFW
```bash
sudo ufw enable
```

## Allow the Web Application on Port 8080
```bash
sudo ufw allow 8080/tcp
```

This rule allows incoming TCP traffic to port 8080 for the web application.

## Verify Firewall Rules
```bash
sudo ufw status verbose
sudo ufw status numbered
```

## Why SSH Must Be Allowed Before Enabling UFW

If UFW is enabled before allowing SSH, remote administrators may lose access to the server because SSH connections can be blocked by the firewall's default incoming policy.
