# OpenCore_Intel_i5_10400_Asrock_H470_Steel_Legends_Only_UHD630

# Info PC
```
Main: Asrock H470 Steel Legend
CPU: Intel® Core™ i5-10400
Ram: 16GB (2x8GB - 3000) Gskill Ripjaw
VGA: UHD 630 (Only use graphic onboard)
Card Wifi + Blutooth: WiFi Intel AX200 802.11ax (2400Mbps) Wi-Fi 6 - Bluetooth 5.0
```
# Reference Hardware
- https://www.asrock.com/mb/Intel/H470%20Steel%20Legend/

# Guide Hackintosh + OpenCore
- https://dortania.github.io/OpenCore-Desktop-Guide

# Version Hackintosh + OpenCore (OpenCore 0.6.7 - macOS Catalina)
- https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.7

# Everything Works
- Continuity:
    - Handoff
    - iMessage (use GenSMBIOS for gen and check coverage at https://coverage.apple.com)
    - Air Drop
- Sleep
- Wake
- Audio (select internal speakers)
- Ethernet
- Bluetooth
- WiFi (Use HeliPort.app, recommend auto start it when login)
- All USB ports (Full 3.0 + 2.0 + type C)

Note: Realtek 8125 Ethernet card required to manually set to 100baseTx (or 1000baseTx if your adapter support) to work
![Realtek 8125 Ethernet](/image/image1.png)

# Note For You
The file config.plist. Please change MLB, SystemSerialNumber, SystemUUID into your code

```
<dict>
  <key>AdviseWindows</key>
  <false/>
  <key>MaxBIOSVersion</key>
  <false/>
  <key>MLB</key>
  <string>xxxxxxxxxxxxxxx</string>
  <key>ProcessorType</key>
  <integer>0</integer>
  <key>ROM</key>
  <data>ESIzRFVm</data>
  <key>SpoofVendor</key>
  <true/>
  <key>SystemMemoryStatus</key>
  <string>Auto</string>
  <key>SystemProductName</key>
  <string>iMac20,1</string>
  <key>SystemSerialNumber</key>
  <string>xxxxxxxxxxxxxxx</string>
  <key>SystemUUID</key>
  <string>xxxxxxxx-xxxxx-xxxxx-xxxx-xxxxxxxx</string>
</dict>
```

