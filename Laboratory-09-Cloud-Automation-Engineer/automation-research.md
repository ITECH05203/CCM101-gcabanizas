# Automation Research

## Bash Script
A Bash script is a plain text file containing a series of shell commands that
run in order, so a task can be repeated without typing each command by hand.
The first line, `#!/bin/bash` (the shebang), tells Linux which program should
interpret the file, in this case the Bash shell, so the script runs correctly
when executed directly.

## Variables
Variables store a value under a name, like `$BACKUP_DIR`, so the script can
reuse it in many places. If the folder path ever changes, I only edit it once
at the top instead of hunting through the whole script, which saves time and
avoids typos.

## Cron Job
A cron job is a task that the Linux cron scheduler runs automatically at a
set time or interval, defined by a line in the crontab. It is essential for
cloud operations because backups, log cleanups, and health checks must happen
reliably on schedule without depending on a person to remember.
