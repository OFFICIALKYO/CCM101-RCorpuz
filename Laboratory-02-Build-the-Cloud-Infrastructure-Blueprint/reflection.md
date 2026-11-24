# Mission Reflection

## 1. Which cloud infrastructure component do you think is the most important? Why?
I believe compute is the most important component because it is where applications actually run. Storage, networking, and identity services all exist to support workloads, and those workloads need CPU and memory to do any work. In the KillerCoda server, the CPU cores from `nproc` and the RAM from `free -h` determine how much the system can handle. However, I also learned that the components depend on each other, so a weakness in any one of them affects the whole system.

## 2. How does Linux support cloud computing?
Linux is the foundation of most cloud servers because it is open source, stable, lightweight, and highly configurable. Cloud providers can run it without licensing costs and customize it for large-scale operations. It also works well with automation through the command line, and it powers technologies such as virtual machines and containers. The KillerCoda environment showed this directly, since I could inspect the whole server using only terminal commands like `lscpu`, `df -h`, and `ip addr`.

## 3. Why is technical documentation important before deploying infrastructure?
Documentation gives engineers a clear record of what exists, what is needed, and why design decisions were made. Without it, teams may misconfigure resources, overspend, or struggle to troubleshoot problems later. In this lab, the infrastructure report acted as an assessment that senior engineers could use to plan the final architecture. Good documentation also makes handovers easier when new team members join a project.

## 4. What new skills did you learn during this laboratory activity?
I learned how to investigate a Linux server using commands such as `uname`, `lscpu`, `free`, `df`, and `ip`. I also learned how to map those resources to compute, storage, networking, and operating system components, compare equivalent services across AWS, Azure, and Google Cloud, and design a simple architecture diagram. Writing structured technical documentation in Markdown was another skill that improved.

## 5. How has your GitHub portfolio improved after completing this mission?
My portfolio now has a second organized laboratory folder with reports, screenshots, and a README, committed checkpoint by checkpoint. The commit history shows steady progress, and the consistent structure makes the repository easier for others to read. It now looks more like a professional engineering portfolio than a simple collection of files.
