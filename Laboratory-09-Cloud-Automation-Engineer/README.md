# Mission 9: The Cloud Automation Engineer

## Mission Overview
This activity eliminates the human error behind a client's missed weekly
backups. Acting as a Cloud Automation Engineer, I created a dummy application
directory, wrote a Bash script that compresses and backs it up with a
timestamped filename, made the script executable with `chmod`, tested it, and
prepared the cron schedule that runs the backup every night at 2:00 AM
without anyone pressing a button.

## Objectives
- Understand the fundamental syntax of a Bash shell script, including variables and basic commands.
- Use a command-line text editor (nano) to write and save executable scripts.
- Modify Linux file permissions using the chmod command.
- Understand task scheduling and the syntax of a Linux crontab.
- Document automation code and Cron job configurations using Markdown.
- Complete the final chapter of my GitHub Cloud Computing Portfolio.

## Commands Executed
| Command | Purpose |
|---|---|
| `mkdir app-data` | Create the dummy application data folder |
| `echo "This is critical client data." > app-data/data.txt` | Create a test file representing the client's data |
| `nano backup.sh` | Create and edit the backup script |
| `./backup.sh` | Run the script (first attempt failed with "Permission denied") |
| `chmod +x backup.sh` | Grant execute permission to the script |
| `ls -l backups/` | Verify the compressed backup file was created |
| `crontab -l` | List the current cron jobs |
| `env EDITOR=nano crontab -e` | Open the cron table in the nano editor |

## Skills Learned
Writing a Bash script with variables, command substitution, and `tar`
compression; setting file permissions with `chmod`; testing a script and
verifying its output; and scheduling a recurring task with a cron expression.
I also practiced documenting code and its schedule clearly enough for a
client's IT team to maintain.
