# Backup Script Guide

## 1. Purpose

The `backup.sh` script automates the backup of the application's data directory. It creates a backup folder when needed, generates a timestamp, and compresses the application data into a `.tar.gz` archive.

## 2. Full Bash Script

```bash
#!/bin/bash
# Automated Backup Script for CloudNova Technologies

SOURCE_DIR="app-data"
BACKUP_DIR="backups"
TIMESTAMP=$(date +"%Y%m%d_%H%M%S")

echo "Initiating automated backup..."

# Create the backup directory if it does not exist
mkdir -p $BACKUP_DIR

# Compress the source directory into a tarball (.tar.gz)
tar -czf $BACKUP_DIR/backup_$TIMESTAMP.tar.gz $SOURCE_DIR

echo "Backup completed successfully at $TIMESTAMP!"
```

## 3. File Permissions

The command `chmod +x backup.sh` gives the script executable permission. This allows Linux to run the script using `./backup.sh` instead of opening it as a text file.

## 4. Cron Job Configuration

The Cron expression used in this activity is:

```cron
0 2 * * * /root/backup.sh
```

### Breakdown of the Five Time Fields

| Field | Value | Explanation |
|---|---|---|
| Minute | `0` | Runs at minute zero |
| Hour | `2` | Runs at 2:00 AM |
| Day of Month | `*` | Runs every day of the month |
| Month | `*` | Runs every month |
| Day of Week | `*` | Applies to every day of the week |

This schedule runs the backup script every day at 2:00 AM, according to the system's local time and assuming the script path is correct.

## 5. Verification Commands

```bash
./backup.sh
ls -l backups/
tar -tzf backups/backup_*.tar.gz
crontab -l
```

These commands run the backup, check the generated archive, inspect its contents, and display the installed Cron schedule.
