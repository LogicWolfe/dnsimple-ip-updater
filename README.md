# dnsimple-ip-updater
Private IP address dynamic DNS entry creation for DNSimple.

## Example Crontab
```
SHELL=/bin/zsh
PATH=/usr/local/sbin:/usr/local/bin:/sbin:/bin:/usr/sbin:/usr/bin

# m h  dom mon dow   command
* * * * * . $HOME/.credentials.zsh; . $HOME/repos/dnsimple-ip-updater/.rvmrc; $HOME/repos/dnsimple-ip-updater/dnsimple-ip-updater 2>&1 | /usr/bin/logger -t dnsimple-ip-updater
```
