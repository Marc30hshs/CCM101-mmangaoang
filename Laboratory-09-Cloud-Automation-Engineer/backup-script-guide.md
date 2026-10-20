
# Backup Script Guide

## 1. Backup Script Code

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="/root/app-data"
BACKUP_DIR="/root/backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

mkdir -p "$BACKUP_DIR"

tar -czf "$BACKUP_DIR/backup_$TIMESTAMP.tar.gz" "$SOURCE_DIR"

echo "Backup completed successfully at $TIMESTAMP!"
```

## 2. File Permissions

The `chmod +x backup.sh` command gives the script executable permission. This allows Linux to run the script as a program.

## 3. Cron Job Configuration

```cron
0 2 * * * /root/backup.sh
```

### Cron Schedule Breakdown

| Field | Value | Meaning |
|---|---|---|
| Minute | 0 | At minute zero |
| Hour | 2 | At 2 AM |
| Day of Month | * | Every day of the month |
| Month | * | Every month |
| Day of Week | * | Every day of the week |

The Cron job automatically runs the backup script every day at 2:00 AM.

## 4. Backup Verification

The `ls -lh /root/backups/` command displays the generated backup files. The `.tar.gz` extension indicates a compressed archive.
