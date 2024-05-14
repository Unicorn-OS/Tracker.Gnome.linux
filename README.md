# Tracker.Gnome
Home: https://tracker.gnome.org/

# Clean space:
>If the Tracker Miner FS database is using a lot of disk space, you can run `tracker3 reset --filesystem` to delete everything stored there.


# disableTracker.linux
sch: https://www.google.com/search?q=linux+cache%2Ftracker3

## Doc:
https://tracker.gnome.org/faq/
>**How can I disable Tracker in GNOME?**  
>In case of a bug you may need to temporarily stop Tracker Miner FS indexing. The simplest way is to edit the configuration so that no directories are indexed. This should bring resource usage to zero.

## alt:
discuss: https://askubuntu.com/questions/1487330/what-is-a-tracker3-folder-inside-home-cache-is-it-safe

disable:
```
systemctl --user mask tracker-extract-3.service tracker-miner-fs-3.service tracker-miner-rss-3.service tracker-writeback-3.service tracker-xdg-portal-3.service tracker-miner-fs-control-3.service
tracker3 reset -s -r
```
