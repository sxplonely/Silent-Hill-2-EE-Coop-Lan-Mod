# Silent-Hill-2-EE-Coop-Lan-Mod
SH2Coop is a cooperative multiplayer mod for Silent Hill 2: Enhanced Edition, allowing up to 4 players to experience James Sunderland's main story together. Features LAN multiplayer via Radmin VPN or Hamachi, synchronized gameplay, shared progression, and individual inventories. Currently supports Chapter 1 only. Further on, a P2P server, including the chapter on Maria.


Installation Guide

(You should use Radmin VPN or a similar alternative to play with your friends remotely.)
1. Close the game. Back up your save files and any previous version of the mod, if present.
2. Extract ALL contents of this ZIP file into the folder containing `sh2pc.exe`. You should end up with `SH2Coop.asi` located next to the `.exe` file, and a `plugins/SH2Coop` folder. Do not place the `.asi` file inside the `plugins/SH2Coop` folder.
3. In your existing `d3d8.ini` file, under the `[Plugins]` section, ensure that `LoadPlugins = 1` and `LoadFromScriptsOnly = 0` are set. Also, enable `d3d8to9 = 1` under the `[DirectX]` section to allow the ImGui lobby to appear. Do not replace the entire `d3d8.ini` file; instead, locate the existing keys—do not create duplicates. If these keys appear in a different section, keep them in their original location.
4. Ensure there are no duplicate copies of `SH2Coop.asi` in other directories scanned by your loader. You do not need any additional ASI loaders, Xidi, `dinput8.dll`, or camera mods to run SH2Coop.
5. Launch `sh2pc.exe`. Select "MULTIPLAYER" from the title menu or press F8; the lobby should then appear. You can use `Verify-Install.ps1` to check your files and requirements without making any modifications.
<img width="460" height="107" alt="image" src="https://github.com/user-attachments/assets/392bf195-5601-40fb-ba1e-67df856cde44" />
<img width="456" height="176" alt="image" src="https://github.com/user-attachments/assets/fc17a4d4-4eaa-4c5d-b1be-91a1dfb7bde9" />
Requires Enhanced Edition
