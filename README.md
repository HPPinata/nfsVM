# nfsVM
This script was created to bring up a simple NFS share in XCP-ng without having to pass through an entire drive controller. It creates a VM running openSUSE MicroOS to manage a simple export.

## Usage:
```
wget https://raw.githubusercontent.com/HPPinata/nfsVM/main/createNFS.bash
cat createNFS.bash #look at the things you download
bash createNFS.bash
```

When the script completes the VM shuts down. After the next startup the NFS share should be reachable on the IP address your DHCP server assigned to the VM (or via the hostname "nfsshare").
