# unixcommands
Unix Commands

Remove all .DS_Store files
```bash
sudo find / -name ".DS_Store" -depth -exec rm {} \;
```

Disable .DS_Store files
```bash
defaults write com.apple.desktopservices DSDontWriteNetworkStores true
```

Open all jpg files in the current subfolders 
```bash
find . -name "*.jpg" | xargs open
```

Flush OSx DNS
```bash
sudo dscacheutil -flushcache; sudo killall -HUP mDNSResponder; say DNS cache flushed 
```
