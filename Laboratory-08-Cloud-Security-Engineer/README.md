# Laboratory 8: Mission 8 – The Cloud Security Engineer

## Mission Overview
In this mission, I acted as a Cloud Security Engineer at CloudNova Technologies. I deployed an Nginx web application in a KillerCoda Ubuntu Playground, then secured the server using the Uncomplicated Firewall (UFW) with a Default Deny policy. Only SSH (port 22) and the web application (port 8080) were allowed through.

## Objectives
- Understand the Attack Surface and the Principle of Least Privilege (PoLP).
- Perform a basic security audit of active network ports on a Linux server.
- Configure UFW with a Default Deny policy.
- Implement granular port management to allow SSH and HTTP traffic.
- Document firewall rules and security best practices using Markdown.
- Continue expanding my GitHub Cloud Computing Portfolio.

## Commands Executed
```bash
# Deploy the application
docker run -d --name secure-web-app -p 8080:80 nginx
curl http://localhost:8080

# Build the firewall
sudo ufw allow ssh
sudo ufw default deny incoming
sudo ufw default allow outgoing
sudo ufw enable
sudo ufw status verbose

# Granular port management
sudo ufw allow 8080/tcp
sudo ufw status numbered
curl http://localhost:8080
```

## Skills Learned
- Running a containerized Nginx web server with Docker.
- Verifying services using curl.
- Configuring UFW with a Default Deny policy.
- Allowing specific ports (SSH and 8080/tcp) and checking rules.
- Applying PoLP and reducing the attack surface of a server.
- Documenting technical work in Markdown and using Git/GitHub.

## Files
- [security-audit-report.md](security-audit-report.md)
- [firewall-configuration.md](firewall-configuration.md)
- [reflection.md](reflection.md)
- [screenshots/](screenshots/)
