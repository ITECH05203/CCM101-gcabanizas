# Reflection

## 1. How does a host-based firewall protect a server even if the physical network perimeter is breached?
A host-based firewall runs on the server itself, so it keeps filtering traffic
even if an attacker gets past the network perimeter, such as a router or cloud
security group. It adds another layer of defense in depth: each machine
decides for itself which connections to accept. If one machine on the network
is compromised, the firewalls on the others can still stop the attacker from
moving sideways.

## 2. Why is managing open network ports critical to reducing a server's attack surface?
Every open port is a service listening for connections, and every listening
service is a possible entry point if it has a bug or a weak password. The
attack surface is the sum of all those entry points, so closing every port
that isn't needed shrinks what an attacker can probe. In this lab only SSH and
port 8080 were open, which follows the Principle of Least Privilege.

## 3. In a real enterprise environment, why is it dangerous to leave a database port (like 3306 for MySQL) open to the public internet?
A database holds an organization's most valuable data, such as customer
records and credentials. If port 3306 is open to the internet, automated
scanners will find it within minutes and attempt brute-force logins or exploit
known MySQL vulnerabilities. Databases should only be reachable from the
application servers that need them, over a private network.

## 4. How did completing this mission change your perspective on how easily a server can be compromised?
Before this lab I assumed a server had to be specifically targeted to be at
risk. Seeing that a freshly deployed server had no firewall rules at all showed
me that an unprotected machine is exposed from the moment it is online.
[Add one sentence in your own words about what surprised you.]

## 5. How does your GitHub portfolio currently look with eight completed missions?
With eight missions complete, my portfolio covers [list the areas you have
completed, such as Linux basics, infrastructure, containers, monitoring, and
security]. Each lab folder follows a similar documentation structure, so the
repository reads like a real engineering portfolio. [Describe in your own
words how it looks to you.]
