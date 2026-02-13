# Auto Backup Script

This repository contains an automated backup script for your system. The script logs its activities and can be managed via crontab.

## Files

- **auto_backup.sh**  
  The main backup script located at `/home/kadal/auto_backup.sh`.

- **auto_backup.log**  
  Log file that records backup activity, located at `/home/kadal/auto_backup.log`.

## Usage

### Check Logs

To view the backup log:

```bash
cat /home/kadal/auto_backup.log
```

### Run Backup Manually (Commit)

To manually run the backup script:

```bash
/home/kadal/auto_backup.sh
```


### Crontab Management

View Current Cron Jobs

```bash
crontab -l
```

Edit Cron Jobs

```bash
crontab -e
```


Add or modify the cron job to schedule automatic backups as needed. Example to run the backup hourly:

```bash
0 * * * * /home/kadal/auto_backup.sh
```


### Permissions

Make sure the backup script has execute permissions:

```bash
chmod +x /home/kadal/auto_backup.sh
```

