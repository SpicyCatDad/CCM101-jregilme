# Reflection

Monitoring the host server's resources is essential even when the containers appear to be working properly. Every container relies on the host machine's available resources. Even if a container is configured correctly, it can still encounter problems when the host runs out of memory or disk space. This shows that container performance depends heavily on the system supporting it.

If a user reported being unable to log in, I could use `docker logs` to examine the requests and events recorded by the web server around the time the issue occurred. By checking for failed requests, server-side errors, and unusual activity, I could gather evidence to help determine whether the problem originated from the client, network, or application.

Logs and metrics provide different types of information. Logs, as examined in Checkpoint 4, record individual events with details such as timestamps and request information, helping explain what happened. Metrics, as observed in Checkpoint 5, provide numerical data such as CPU usage, memory consumption, and network activity. These measurements help identify performance changes and possible issues, while logs provide additional details for investigating their causes.

Large enterprises that manage thousands of containers need centralized monitoring systems instead of checking every container individually. Tools such as Prometheus collect and store performance metrics over time, while Grafana presents the information through dashboards and visualizations. These tools allow engineers to monitor multiple servers and containers more efficiently than relying on commands like `docker stats` alone.

Through this laboratory activity, I have improved my ability to troubleshoot Linux environments using actual system data. Rather than relying only on visible symptoms, I have learned to check resource usage with `free`, `df`, and `top`, then compare those findings with container logs and performance metrics. This approach helps me make more informed decisions and identify potential problems before concluding what caused them.
