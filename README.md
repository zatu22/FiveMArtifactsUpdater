# FiveM Artifact Updater Script Manually and Automatically

#Linux only
Update.sh:

1. Copy update.sh to your server where alpine and run.sh is located
2. Close fivem & screen  (when screen name is not txAdmin)
3. bash update.sh
4. follow instruction

You can run update.sh at anytime again, screen get automatically closed and reopen after update and you will always have a backup of last artifact version in backup folder

#Linux only
cronjobupdate.sh:
(No interaction necessary - always fetch LATEST OPTIONAL)

1. Copy cronjobupdate.sh to your server where alpine and run.sh is located
2. Close fivem & screen  (when screen name is not txAdmin)
3. bash cronjobupdate.sh
4. Run update automatically: 
5. ```crontab -l | { cat; echo "30_4_*_*_0 /bin/bash "path/to/server/cronjobupdate.sh""; } | crontab -```
6. (optional) enable log in cronjobupdate.sh
7. Every Sunday 4.30am artifact update starts automatically
