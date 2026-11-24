# Mission Reflection

**1. How does a host-based firewall protect a server even if the physical network perimeter is breached?**
A host-based firewall runs on the server itself, so it filters traffic no matter what network the machine sits in. If an attacker gets past the network perimeter or onto the same internal network, the firewall still drops any packet that does not match an allowed rule. This provides defense in depth because no single layer is trusted completely.

**2. Why is managing open network ports critical to reducing a server's attack surface?**
Every open port is a running service that someone can probe, and every service may have bugs or weak passwords. Closing the ports that are not needed shrinks the attack surface and gives attackers fewer entry points to scan and exploit. In this lab, only SSH and port 8080 were opened, and everything else was blocked by default.

**3. In a real enterprise environment, why is it dangerous to leave a database port (like 3306 for MySQL) open to the public internet?**
An open port 3306 exposes the database directly to the internet, where bots constantly scan for it and attempt brute-force logins or exploit known MySQL vulnerabilities. A breach could lead to stolen or deleted customer data, which has legal and financial consequences. Databases should stay on a private network and be reachable only by the application server.

**4. How did completing this mission change your perspective on how easily a server can be compromised?**
Before this mission, I assumed a server needed a sophisticated attack to be compromised. I learned that a server without a firewall is exposed by default, and that good security starts with simple steps like Default Deny and allowing only what is needed. I also saw how one wrong order of commands, like enabling the firewall before allowing SSH, can lock out the administrator.

**5. How does your GitHub portfolio currently look with eight completed missions?**
My portfolio now has eight laboratory folders, each with a README, documentation, and screenshots as evidence. It shows steady progress from basic cloud concepts to cloud security, and the consistent structure makes it easy to review. I will keep committing after every checkpoint to maintain a clean history.
