# Automation Research

## Bash Script
A Bash script is a text file that holds a list of commands, so I can run them
all at once instead of typing each one. The first line, `#!/bin/bash`, is
called the shebang, and it tells Linux to run the file using the Bash shell.

## Variables
A variable stores a value under a name, like `$BACKUP_DIR`, so I can reuse it
anywhere in the script. If the folder path changes, I only have to fix it in
one place instead of editing every line, which also helps me avoid typos.

## Cron Job
A cron job is a task that Linux runs by itself at a time I choose, set up with
a line in the crontab. It's important in cloud operations because jobs like
backups need to happen on schedule, and I can't count on someone remembering
to run them.
