# Laboratory Activity 7: The Cloud Operations Engineer

## Mission Overview
This activity simulates a baseline health check on a production server ahead
of a large marketing campaign. Acting as a Cloud Operations Engineer, I
measured the host's memory, disk, and CPU, deployed a containerized Nginx web
server, generated normal and failing web traffic, and used application logs
and real-time container metrics to confirm the infrastructure is ready for a
surge in users.

## Objectives
- Utilize native Linux command-line tools to monitor host CPU, memory, and disk capacity.
- Deploy a web container and track its real-time performance using Docker metrics.
- Generate web traffic and extract application access logs for analysis.
- Translate raw performance data into a readable technical report using Markdown.
- Continue expanding a professional GitHub Cloud Computing Portfolio.

## Monitoring Commands Executed
| Command | Purpose |
|---|---|
| `free -h` | Check total and used memory (RAM) on the host |
| `df -h` | Check disk capacity and available storage |
| `top` | View active processes and live CPU load |
| `docker run -d -p 8080:80 --name client-website nginx` | Deploy the client's Nginx web server in the background |
| `curl http://localhost:8080` | Simulate a user visiting the website (sent three times) |
| `curl http://localhost:8080/hidden-admin-page` | Request a non-existent page to generate an HTTP 404 error |
| `docker logs client-website` | Retrieve the container's application access logs |
| `docker stats` | View live CPU, memory, and network usage of the container |

## Skills Learned
Establishing a host performance baseline with standard Linux tools;
deploying a containerized web server; simulating normal and failing user
traffic; reading application logs to find specific HTTP status codes;
interpreting real-time container metrics; and presenting observability data
in a clear Markdown report.
