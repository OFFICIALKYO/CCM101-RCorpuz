# Container Observability

## Checkpoint 4 - Application Logging

### Command Executed

```bash
docker logs client-website
```

### HTTP 404 Error Log Entry

```text
172.17.0.1 - - [05/Oct/2026:05:34:41 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

### Why Application Logs Are Vital for Troubleshooting

Application logs are important because they record website activities, requests, errors, and timestamps, helping engineers understand what happened when a problem occurred. By checking these logs, we can identify issues like HTTP 404 errors and troubleshoot them faster instead of guessing the cause of the problem.

### Short Explanation

The log shows that a user tried to access `/hidden-admin-page`, but the server returned an HTTP 404 error because the requested page or resource was not found. This helps us understand how Docker logs can be used to identify failed requests and monitor application activities.

## Checkpoint 5 - Container Metrics

### Command Executed

```bash
docker stats --no-stream client-website
```

### Container Monitoring Results

- **Container Name:** client-website
- **CPU Usage:** 0.00%
- **Memory Usage:** 2.738MiB / 1.859GiB
- **Memory Percentage:** 0.14%

### Short Explanation

I used the `docker stats` command to monitor the CPU and memory usage of my running container. Based on the results, the container was using 0.00% CPU and 2.738MiB of memory, which is only 0.14% of the available memory limit. This shows that the container was consuming very few resources at the time of monitoring.

### What I Learned

In this checkpoint, I learned how to monitor Docker containers using `docker logs` and `docker stats`. These commands help me identify application errors and check resource consumption. I also learned that monitoring is important because it helps cloud engineers detect possible problems and maintain the performance of applications running inside containers.
