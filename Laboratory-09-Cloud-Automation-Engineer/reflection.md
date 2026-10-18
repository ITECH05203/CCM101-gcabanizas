# Reflection

## 1. Why is automation critical when managing hundreds of cloud servers?
Managing hundreds of servers by typing commands one at a time is too slow and
easy to get wrong. Automation lets a single script do the same task
identically on every machine, saves enormous amounts of time, and removes
human errors like forgetting a backup. It also makes work repeatable, so the
result is consistent no matter who runs it.

## 2. What are the potential dangers of automation?
Automation multiplies mistakes just as efficiently as it multiplies
successes. A destructive typo in a script scheduled on 1,000 servers, such as
deleting the wrong directory, would damage every one of them at once, possibly
overnight with nobody watching. That is why scripts should be tested on a
single machine first, reviewed, and run only with good backups in place.

## 3. How did writing a Bash script differ from creating a Docker Compose YAML file (Mission 6)?
A Bash script is a list of commands executed step by step, so it describes
how to do a task. A Docker Compose YAML file is declarative: it describes the
desired state of the services and lets Docker work out how to create it. Bash
felt like giving instructions, while YAML felt like filling in a specification.

## 4. Review your entire GitHub repository from Laboratory 1 to Laboratory 9. How has your understanding of Cloud Computing transformed over the course of this semester?
At the start, the cloud felt like an abstract idea. Moving from Linux basics
to infrastructure, containers, monitoring, and automation showed me that the
cloud is layers of servers, networking, and software that engineers manage and
document. [Add one or two sentences about your own experience across the labs.]

## 5. Which role did you enjoy the most and why?
[Choose your role.] I enjoyed the [role] work the most because [your honest
reason, such as which tasks you liked doing hands-on and what you found
interesting or satisfying about them].
