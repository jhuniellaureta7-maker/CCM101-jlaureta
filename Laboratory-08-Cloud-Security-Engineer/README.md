
## Mission Overview
Congratulations! I was given a position on CloudNova Technologies' Cloud Security Team because of my proactive approach to system monitoring.

Leaving a server unprotected in cloud computing can result in data breaches and brute-force attacks. I used a host-based firewall to protect a server in this mission, putting the security principles from Chapter 8 into practice.

I set up the Uncomplicated Firewall (UFW), checked the server's network ports, and deployed a Nginx web application using the KillerCoda Playground. Only the necessary traffic for SSH and the web application on port 8080 was permitted after I implemented the Default Deny policy.

## Objectives
- Understand the Principle of Least Privilege and attack surface.
- Configure a Default Deny firewall policy.
- Allow SSH traffic for administration.
- Allow TCP traffic on port 8080 for the web application.
- Verify firewall rules and document the security configuration.

## Commands Executed
```bash
docker run -d -p 8080:80 --name secure-web-app nginx
docker ps
curl -i http://localhost:8080/
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose
sudo ufw allow 8080/tcp
sudo ufw status numbered
```

## Skills Learned
I learned how to deploy an Nginx container, check the rules of the firewall, configure a Default Deny policy, allow specific traffic, and document basic Linux server security policies.
