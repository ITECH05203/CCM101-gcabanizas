# Backup Script Guide

This guide documents the automated backup solution so the client's IT team
can understand, maintain, and reproduce it.

## The Script (`backup.sh`)
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

## What `chmod +x` Did
By default, a newly created text file is not allowed to run as a program, which
is why `./backup.sh` first returned "Permission denied." The `chmod +x
backup.sh` command added the execute permission to the file, so Linux now
allows it to be run as a program.

## The Cron Expression
```
0 2 * * * /root/backup.sh
```

| Field | Value | Meaning |
|---|---|---|
| Minute | `0` | At minute 0 of the hour |
| Hour | `2` | At 2 AM (24-hour clock) |
| Day of Month | `*` | Every day of the month |
| Month | `*` | Every month |
| Day of Week | `*` | Every day of the week |

Together, this runs `/root/backup.sh` every night at exactly 2:00 AM.
