# Mission Reflection

**1. Why is automation critical when managing hundreds of cloud servers?**
Manual work does not scale. Typing the same commands on hundreds of servers takes hours and almost guarantees that someone skips a step or makes a typo. A script or cron job runs the same way every time, so backups, updates, and checks happen consistently without relying on a person to remember them.

**2. What are the potential dangers of automation?**
Automation multiplies mistakes as efficiently as it multiplies good work. If a script has a destructive typo, such as a wrong path in a delete command, and it is scheduled on 1,000 servers, the damage happens everywhere at the same time, often at 2:00 AM when nobody is watching. Scripts should be tested on one machine first, reviewed, and rolled out gradually, with separate backups in place.

**3. How did writing a Bash script differ from creating a Docker Compose YAML file (Mission 6)?**
Docker Compose YAML is declarative: I describe the end state I want, and Docker figures out how to reach it. Bash is imperative: I write each step in order and I am responsible for the logic, variables, and permissions like `chmod +x`. Bash gives more control, but it also gives more room for mistakes.

**4. How has my understanding of Cloud Computing transformed this semester?**
In Laboratory 1, cloud computing felt like a buzzword. By Laboratory 9, I had used Git and Markdown, designed infrastructure, explored different cloud providers, worked with containers, deployed services, monitored operations, secured systems, and automated tasks. I now see the cloud as many connected engineering roles, and my repository shows that progress from basic commands to real workflows.

**5. Which role did I enjoy the most and why?**
I enjoyed the Cloud Automation Engineer role the most. Seeing a script and one cron line replace a manual task that people forget felt practical, and it connects to my IoT and development projects where repeated tasks can be automated too.
