# Security Audit Report

## Chapter 8 Security Concepts

### The Principle of Least Privilege (PoLP)
The Principle of Least Privilege means giving a user, application, or service only the minimum permissions it needs to do its job, and nothing more. It is important for cloud user accounts because if an account is stolen or misused, the damage is limited to what that account was allowed to do. It also reduces the risk of accidental changes or deletions by authorized users.

### Attack Surface
The attack surface of a virtual machine is the total number of points where an attacker can try to get in or extract data. This includes open network ports, running services, installed software, and user accounts. The more ports and services that are exposed, the larger the attack surface and the more opportunities there are for an attack.

### Default Deny Policy
A Default Deny policy blocks all incoming traffic unless a rule explicitly allows it. It is safer than blocking specific hackers one by one because attackers constantly change their IP addresses and tools, so a blocklist can never be complete. With default deny, anything unknown is automatically blocked, and only the services we intentionally allow are reachable.
