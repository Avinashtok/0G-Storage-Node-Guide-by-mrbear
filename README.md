# 🚀 0G Storage Node Guide by Mrbear

📦 Use this snapshot to sync your node faster!

---

### ✅ Snapshot Info
- **Block**: 3507655
- **File**: [Download Here (flow_db-3507655.tar.gz)](https://github.com/Avinashtok/0g-fast-sync/releases/download/backup-3507655/flow_db-3507655.tar.gz)
- **SHA256 Checksum**:  

---

### ⚙️ Commands for Fast Sync

```bash
# Stop Node
sudo systemctl stop zgs

# Remove Old DB
rm -rf $HOME/0g-storage-node/run/db/flow_db

# Download Snapshot
wget -O flow_db.tar.gz https://github.com/Avinashtok/0g-fast-sync/releases/download/backup-3507655/flow_db-3507655.tar.gz

# Extract it
tar -xzvf $HOME/0g-storage-node/run/db/flow_db.tar.gz -C $HOME/0g-storage-node/run/db/

# Restart Node
sudo systemctl restart zgs
