## Fast Sync Steps

1. Stop your node:
```bash
sudo systemctl stop zgs

Remove existing DB folder:
rm -rf $HOME/0g-storage-node/run/db/flow_db

Download snapshot:

wget -O flow_db.tar.gz https://github.com/Avinashtok/0G-fast-sync/releases/download/backup-3507655/flow_db-3507655.tar.gz
