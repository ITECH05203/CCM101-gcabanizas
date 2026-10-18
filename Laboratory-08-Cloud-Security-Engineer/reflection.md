# Reflection

## 1. How a host-based firewall protects a server
A host-based firewall sits on the server itself, so it still protects the
machine even if someone gets past the network perimeter. It works like a lock
on every door inside a building, not just the front gate. If one machine gets
compromised, the other servers' firewalls can still stop the attacker from
spreading.

## 2. Why managing open ports matters
Every open port is a service listening for connections, and each one could be
a way in if it has a bug or a weak password. Closing the ports I don't need
makes the attack surface smaller, so there is less for an attacker to try. In
this lab I only left SSH and port 8080 open, which matches the Principle of
Least Privilege.

## 3. Why an open database port is dangerous
A database like MySQL holds the most valuable data, such as customer records.
If port 3306 is open to the internet, automated scanners can find it quickly
and try brute-force logins or known exploits. Databases should only be
reachable by the application servers that need them, over a private network.

## 4. How this mission changed my perspective
Before this lab, I thought a server only got attacked if someone targeted it
on purpose. This mission showed me that a server with no firewall is exposed
as soon as it goes online, and that securing it takes only a few commands. It
made me trust default settings a lot less.

## 5. How my portfolio looks with eight missions
With eight missions done, my portfolio now covers Linux basics, cloud
infrastructure, containers, monitoring, and security. Each lab folder has a
README, documentation, and screenshots, so it looks more like a real
engineering portfolio than a pile of assignments.
