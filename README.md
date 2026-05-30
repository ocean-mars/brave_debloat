# Brave Debloater

**A single Linux JSON file to safely debloat [Brave Browser](https://brave.com/).**  

This project disables **Brave AI, Rewards, Wallet, VPN, Telemetry, News, Talk, Speedreader, Playlist**, and other non-essential features, giving you a **cleaner, faster, and more private browsing experience**.  

> **Note:** Sync & DoH setting is **left untouched**. 

## Features
- Disable Brave AI (Chat, Leo, Summarizer)  
- Turn off Rewards, Wallet, VPN, and Tor  
- Disable Telemetry (P3A, Stats Ping, Web Discovery)  
- Remove News, Talk, Speedreader, Playlist, and Wayback Machine  
- Disable Autofill, Password Manager, and Translation  
- Shields, Sync & DoH untouched

## Linux
1. Create the managed policies directory (if it doesn't exist): \
   `sudo mkdir -p /etc/brave/policies/managed/`
2. Copy `policies.json` into the directory: \
   `cd /etc/brave/policies/managed/` \
   `sudo curl -L -O https://raw.githubusercontent.com/ocean-mars/brave_debloat/refs/heads/main/policies.json`
3. Restart Brave to apply the changes. Verify applied policies by visiting: `brave://policy/`

## Flatpak Version
1. Create the managed policies directory (if it doesn't exist): \
   `sudo mkdir -p /etc/brave/policies/managed/`
2. Copy `policies.json` into the directory: \
   `cd /etc/brave/policies/managed/` \
   `sudo curl -L -O https://raw.githubusercontent.com/ocean-mars/brave_debloat/refs/heads/main/policies.json`
3. Grant the Flatpak app access to the policies directory: \
   `sudo flatpak override --filesystem=/etc/brave/policies/managed com.brave.Browser`
4. Restart Brave to apply the changes. Verify applied policies by visiting: `brave://policy/`

## More
- To learn more and understand about policy settings, visit [Instinctive](https://instinctive.app/chromesettings/)
## Credits
- mattvisa
- MulesGaming
