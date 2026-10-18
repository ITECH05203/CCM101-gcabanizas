# Mission 9: The Cloud Automation Engineer

## Mission Overview
In this lab, I helped fix a client's problem of forgetting weekly backups. I
made a dummy `app-data` folder, wrote a Bash script that compresses it into a
timestamped backup, made the script executable with `chmod`, tested it, and
set up a cron schedule so it runs every night at 2:00 AM without anyone
pressing a button.

## Objectives
- Understand the basic syntax of a Bash script, including variables and commands.
- Use the nano text editor to write and save scripts.
- Change Linux file permissions using `chmod`.
- Understand task scheduling and the syntax of a crontab.
- Document automation code and cron job settings in Markdown.
- Complete the final chapter of my GitHub Cloud Computing Portfolio.

## Commands Executed
| Command | Purpose |
|---|---|
| `mkdir app-data` | Create the dummy application data folder |
| `echo "This is critical client data." > app-data/data.txt` | Create a test file to represent the client's data |
| `nano backup.sh` | Write the backup script |
| `./backup.sh` | Run the script (the first try showed "Permission denied") |
| `chmod +x backup.sh` | Make the script executable |
| `ls -l backups/` | Check that the compressed backup file was created |
| `crontab -l` | View the current cron jobs |
| `env EDITOR=nano crontab -e` | Edit the cron table using nano |

## Skills Learned
I learned how to write a Bash script with variables and the `tar` command,
how to give a file permission to run with `chmod`, and how to test a script
and check its results. I also learned how to schedule a task with a cron
expression and how to document it so someone else can follow it.
