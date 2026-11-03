# Laboratory Activity 9: Mission 9 – The Cloud Automation Engineer

## Mission Overview
This laboratory focuses on reducing manual work and preventing human errors through task automation. It involves creating a Bash script that compresses and backs up application data automatically, then configuring a cron job to execute the script every day at 2:00 AM without requiring manual intervention.

## Objectives
- Learn the basic structure and syntax of Bash scripts, including variables and commands
- Create, edit, and save an executable script using the nano text editor
- Apply the appropriate file permissions using `chmod`
- Understand how Linux schedules automated tasks through crontab
- Record automation scripts and scheduling configurations using Markdown

## Commands Executed
- `mkdir app-data` / `echo "..." > app-data/data.txt` — created a sample directory containing test application data
- `nano backup.sh` — created and edited the Bash backup script
- `chmod +x backup.sh` — assigned execute permission to the script
- `./backup.sh` — executed the script to generate a compressed `.tar.gz` backup file
- `crontab -e` — opened the cron configuration file and added a schedule to run the backup script daily at 2:00 AM using `0 2 * * * /root/backup.sh`
- `crontab -l` — displayed the current cron entries to confirm the scheduled task was saved

## Skills Learned
- Creating and running Bash scripts to automate Linux operations
- Assigning and modifying file permissions through `chmod`
- Setting up recurring tasks using the Linux cron scheduler
- Understanding crontab scheduling expressions and their purpose
- Documenting automation scripts and configurations for easier maintenance and reference
