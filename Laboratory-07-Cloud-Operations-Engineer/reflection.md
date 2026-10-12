# Reflection

## 1. Why is it important to check the host server's resources even if your containers are running perfectly?
Containers do not have their own hardware; they all share the host's CPU,
memory, and disk. A container can look perfectly healthy while the host
quietly runs out of disk space or RAM, and when that happens every container
on the machine can slow down or crash at once. Establishing a baseline
before a traffic surge tells me how much room the server really has.

## 2. If a user complains that they cannot log into a web application, how would the docker logs command help you solve the problem?
The docker logs command would let me see exactly what happened when the user
tried to log in. I could look for error codes such as 401, 403, or 500, match
timestamps to the user's attempt, and check whether the request even reached
the application. That tells me whether the problem is bad credentials, an
application bug, or a crashed service, instead of guessing.

## 3. What is the difference between monitoring logs (Checkpoint 4) and monitoring metrics (Checkpoint 5)?
Logs are a record of individual events, like each HTTP request and its
status code, so they explain what happened and why. Metrics are numbers
measured over time, like CPU percentage and memory usage, so they show how
the system is performing. Logs helped me find the 404 error, while docker
stats showed the container was lightweight.

## 4. How do you think large enterprise companies monitor thousands of containers at the same time?
Large companies cannot check containers one by one. Tools like Prometheus
automatically collect metrics from thousands of containers at regular
intervals and store them, while Grafana turns that data into dashboards and
alerts so teams notice problems quickly.

## 5. How has your ability to troubleshoot Linux environments improved?
My troubleshooting has become more methodical. I now start with the host
baseline using free, df, and top, then check logs with docker logs, then
confirm resource use with docker stats, instead of randomly trying fixes.
