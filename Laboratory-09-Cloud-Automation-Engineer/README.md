# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

This laboratory focuses on automating cloud administration tasks using Bash scripting, Linux file permissions, and Cron scheduling. The main task is to create a script that compresses application data and schedules automatic daily backups.

## Objectives

- Understand basic Bash scripting.
- Create and execute a backup script.
- Use `chmod` to change file permissions.
- Configure a Cron job to run a script automatically.
- Document the automation process using Markdown.

## Commands Executed

```bash
mkdir -p /root/app-data
echo "This is critical client data." > /root/app-data/data.txt
nano /root/backup.sh
chmod +x /root/backup.sh
/root/backup.sh
ls -lh /root/backups/
tar -tzf /root/backups/backup_*.tar.gz
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

- Bash shell scripting
- Linux file permissions
- Automated backup creation
- Cron job scheduling
- Technical documentation using Markdown
- GitHub portfolio management

## Screenshots

- `screenshots/script-execution.png`
- `screenshots/cron-schedule.png`
