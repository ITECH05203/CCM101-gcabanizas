# Container Observability

## HTTP 404 Log Entry
```
172.17.0.1 - - [12/Oct/2026:03:15:15 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are vital for troubleshooting because they record exactly
what happened and when, including the request, the response code, and the
client involved. Without logs, an engineer can only guess why a service
failed instead of tracing the problem to its cause.

## Container Metrics (docker stats)
- **Container:** client-website
- **CPU %:** 0.00%
- **Memory Usage:** 2.734MiB
