# Mission Reflection

In Laboratory 07, I learned how important monitoring is when managing Linux servers and Docker containers. Even if the containers are running properly, we still need to check the host server resources. This is because the server might have high CPU usage, low memory, or almost full storage. If we don't monitor these resources, the containers might become slow or stop working.

If a user complains that they cannot log into a web application, I can use the `docker logs` command to check what is happening inside the container. The logs can show error messages, database connection problems, or application errors. By reading the logs, I can identify the possible cause of the problem and find a solution instead of guessing.

I also learned the difference between monitoring logs and monitoring metrics. Logs show the events and errors happening inside an application, while metrics show the performance of the system, such as CPU usage, memory consumption, and network activity. Both are important because logs help us understand what went wrong, while metrics help us see if the system is performing well.

For large companies that manage thousands of containers, I think they use monitoring tools like Prometheus and Grafana. Prometheus collects performance metrics from different servers and containers, while Grafana displays the collected data using dashboards and graphs. These tools make monitoring easier because engineers don't need to check every container manually.

My troubleshooting skills in Linux have improved because I now know more commands like `top`, `free -h`, `df -h`, `docker logs`, and `docker stats`. Before, I didn't know how to check server performance properly. Now, I can identify possible problems and understand how to fix them. This laboratory helped me become more confident in managing and monitoring cloud environments.
