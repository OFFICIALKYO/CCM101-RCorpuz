# Automation Research: The Language of Automation

## Bash Script
A Bash script is a plain text file containing a series of Linux commands that the Bash shell runs in order, so repetitive tasks can be done automatically instead of typed one by one. The shebang line `#!/bin/bash` at the top tells the system which interpreter (Bash) should be used to run the file.

## Variables
Variables store a value, like a folder path, under a name so it can be reused anywhere in the script. If the path changes, I only edit it once at the top instead of fixing every line, which saves time and prevents typing mistakes. It also makes the script easier to read.

## Cron Job
A cron job is a task that the Linux cron scheduler runs automatically at a set time or interval, based on a schedule written in the crontab. It is essential for cloud operations because backups, updates, and monitoring can run on time every time, even when nobody is logged in.
