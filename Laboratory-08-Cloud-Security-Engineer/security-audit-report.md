# Security Audit Report

## The Principle of Least Privilege (PoLP)
PoLP means a user or account should only get the permissions it really needs
to do its work. I think it matters for cloud accounts because if someone's
account gets hacked, the attacker can only reach what that account was allowed
to touch, so the damage stays small.

## Attack Surface
For a virtual machine, the attack surface is every way someone could try to
get in, like open ports, running services, and user accounts. The more things
a VM leaves open, the more chances an attacker has to find a weak spot, so
keeping it small makes the server safer.

## Default Deny Policy
Default deny means everything coming in is blocked unless I specifically allow
it. It's safer than blocking hackers one by one because there are too many
attackers and they keep changing, while allowing only the few services the
server needs is easy to manage.
