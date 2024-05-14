# disableTracker3.linux
sch: https://www.google.com/search?q=linux+cache%2Ftracker3

discuss: https://askubuntu.com/questions/1487330/what-is-a-tracker3-folder-inside-home-cache-is-it-safe

disable:
```
systemctl --user mask tracker-extract-3.service tracker-miner-fs-3.service tracker-miner-rss-3.service tracker-writeback-3.service tracker-xdg-portal-3.service tracker-miner-fs-control-3.service
tracker3 reset -s -r
```
