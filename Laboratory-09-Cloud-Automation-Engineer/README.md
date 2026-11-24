# Laboratory 09: Cloud Automation Engineer

## Mission Overview
In this mission, I acted as a Cloud Automation Engineer at CloudNova Technologies. The goal was to remove human error from backups by writing a Bash script that compresses an application directory, making it executable, and scheduling it with cron to run every night at 2:00 AM.

## Objectives
- Understand the basic syntax of a Bash script, including variables and commands
- Use nano to write and save a script
- Change file permissions using `chmod`
- Understand task scheduling and crontab syntax
- Document automation code and cron configuration using Markdown
- Complete the final chapter of the GitHub Cloud Computing Portfolio

## Commands Executed
```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh            # Permission denied
chmod +x backup.sh
./backup.sh            # Successful backup
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
0 2 * * * /root/backup.sh
crontab -l
```

## Skills Learned
- Writing Bash scripts with variables and command substitution
- Creating compressed backups with `tar -czf`
- Managing file permissions with `chmod +x`
- Scheduling automated jobs with cron and reading crontab syntax
- Documenting technical work in Markdown

## Files
- [automation-research.md](automation-research.md)
- [backup-script-guide.md](backup-script-guide.md)
- [reflection.md](reflection.md)
- Screenshots: `screenshots/script-execution.png`, `screenshots/cron-schedule.png`
