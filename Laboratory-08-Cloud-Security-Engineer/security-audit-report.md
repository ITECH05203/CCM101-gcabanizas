# Security Audit Report

## The Principle of Least Privilege (PoLP)
The Principle of Least Privilege means giving every user, account, or service
only the minimum permissions it needs to do its job, and nothing more. It is
important for cloud user accounts because if an account is stolen or misused,
the damage is limited to what that account was allowed to access.

## Attack Surface
The attack surface of a virtual machine is the total set of points where an
attacker could try to get in, such as open ports, running services, user
accounts, and installed software. The more services and open ports a VM
exposes, the larger its attack surface and the more chances there are for a
weakness to be exploited.

## Default Deny Policy
A Default Deny policy blocks all incoming traffic unless a rule explicitly
allows it. It is safer than blocking individual hackers because attackers
constantly change addresses and methods, so a block list can never be
complete, while an allow list only admits the few services the server
actually needs.
