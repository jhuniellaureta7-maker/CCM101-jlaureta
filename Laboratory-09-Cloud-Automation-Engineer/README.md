# Laboratory 09 – Cloud Automation Engineer

## Mission Overview

Congratulations! Your ability to secure cloud environments has proven you are ready for the highest level of operations. You have been promoted to the Cloud Automation and DevOps Team at CloudNova
Technologies.

Up until now, you have been acting as a traditional systems administrator—typing commands manually one by one. In large enterprise environments scaling to thousands of servers, manual administration is too slow
and highly prone to human error. To survive at scale, you must learn to automate.

Using the KillerCoda Playground, you will step into the role of a Cloud Automation Engineer. You will learn the basics of Bash shell scripting, create an automated backup routine, assign executable permissions, and configure the Linux Cron scheduler to run your code autonomously.

Remember: If you have to do a task more than twice in the cloud, you should automate it.

## Objectives

- Understand Bash script syntax, variables, and the shebang.
- Create and save a script using the Nano text editor.
- Use `chmod +x` to make a script executable.
- Compress application data into a `.tar.gz` backup file.
- Configure and verify a Cron schedule.
- Document the automation process in the GitHub portfolio.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
./backup.sh
chmod +x backup.sh
ls -l backups/
tar -tzf backups/backup_*.tar.gz
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned

I learned how to construct a Bash script, apply variables, adjust permissions, and make a compressed file of a backup archive. Also, I became familiar with the application of Cron for scheduling recurring tasks and the importance of verifying the integrity of backups and automating configuration documentation.
