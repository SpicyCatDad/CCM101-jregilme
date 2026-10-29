# Laboratory Activity 7: Mission 7 – The Cloud Operations Engineer

## Mission Overview
This laboratory activity focuses on server observability and monitoring. The tasks involve checking the server's initial resource usage, deploying an Nginx web server inside a Docker container, sending successful and unsuccessful HTTP requests, and examining logs and performance metrics to evaluate the server's health and readiness for increased traffic.

## Objectives
- Monitor the server's CPU activity, memory usage, and disk capacity using Linux command-line tools.
- Deploy an Nginx web server in a container and observe its resource consumption.
- Simulate normal and invalid web requests and analyze the resulting access logs.
- Interpret system and container performance data and present the findings in a clear technical report.

## Monitoring Commands Executed
- `free -h` — displays RAM and swap usage.
- `df -h` — checks filesystem capacity and available disk space.
- `top` — monitors CPU activity, running processes, and system resource usage in real time.
- `docker run -d --name client-website -p 8080:80 nginx` — launches an Nginx container and maps port 8080 on the host to port 80 in the container.
- `curl http://localhost:8080` — sends a request to test whether the web server responds normally.
- `curl http://localhost:8080/hidden-admin-page` — requests a nonexistent page to generate an HTTP error response.
- `docker logs client-website` — retrieves the container's logs for request and error analysis.
- `docker stats` — displays live resource usage, including CPU, memory, and network I/O, for running containers.

## Skills Learned
- Establishing a baseline of server performance before deploying applications.
- Generating HTTP requests and interpreting access logs and response status codes.
- Monitoring container resource consumption through Docker's live metrics.
- Distinguishing between **metrics**, which describe system performance, and **logs**, which record application events and requests.
- Using monitoring results to assess server health and identify potential issues before traffic increases.
