# Silent-Hill-2-EE-Coop-Lan-Mod
SH2Coop is a cooperative multiplayer mod for Silent Hill 2: Enhanced Edition, designed for up to 4 players.

Version 34.59-rc1 includes LAN multiplayer and Internet multiplayer through Epic Online Services (EOS), with public rooms and private rooms using four-digit PINs. Cooperative support is implemented for James Sunderland’s main story and Maria’s Born from a Wish scenario.

This is a release candidate. Complete campaign playthroughs and four-player Internet gameplay with this version have not yet been fully validated.
Features
- Up to four players through LAN or EOS.
- Public EOS room browser and private rooms with four-digit PINs.
- Synchronization systems for players, animations, enemies, damage, cinematics, and puzzle progression.
- Individual inventories and consumables. Confirmed puzzle-item use is shared and removes the used puzzle item from players who possess it.
- Cooperative saves stored separately from single-player saves.
- Host-only saving through F9 and red save points.
- Shared checkpoint recovery when a player dies.
- Removal of disconnected players’ characters.
- Four-player room capacity enforcement.
Requirements
- Your own installation of Silent Hill 2 for PC with Enhanced Edition working correctly.
- Windows 10 or 11, 64-bit. The game and mod are 32-bit; the EOS helper is 64-bit.
- Every player must install SH2Coop 34.59-rc1 and use the same Enhanced Edition version.
- Internet access for EOS multiplayer.
The package does not include Silent Hill 2, Enhanced Edition, or a third-person camera mod. Existing camera mods are preserved during installation.

Radmin VPN and Hamachi are not required for EOS. They remain alternatives for playing through the LAN connection mode.
Installation Guide
1. Download SH2Coop-34.59-rc1.zip.
2. Close Silent Hill 2. Back up your saves before updating.
3. Right-click the ZIP and select Extract All. Extract the entire package into a separate folder.
4. Open the extracted folder and run Instalar-SH2Coop.cmd. Do not run it from inside the ZIP.
5. When prompted, enter the game folder containing sh2pc.exe, for example:D:\SH 2
6. Press Enter and wait for the installation-completed message.
The installer verifies package files, backs up replaced files, removes duplicate SH2Coop plugins from loader locations, and updates the existing loader settings:
LoadPlugins = 1
LoadFromScriptsOnly = 0
d3d8to9 = 1
It preserves your saves, controls, camera files, and unrelated configuration settings.

The installed structure should look like this:
Silent Hill 2/
├── sh2pc.exe
├── SH2Coop.asi
└── plugins/
    └── SH2Coop/
        ├── assets/
        ├── bin/
        └── eos.public.ini
Do not rename the payload folder or copy it directly into the game as the installation method. It contains the files used by the installer. Do not install only SH2Coop.asi.
Playing Online Through EOS
1. Launch sh2pc.exe and select MULTIJUGADOR.
2. Select RED: INTERNET (EOS).
3. The host selects CREAR SERVIDOR, then:
   - CREAR SALA PUBLICA: other players find it under SERVIDORES PÚBLICOS, refresh with F5, select it, and join.
   - CREAR SALA PRIVADA: the host shares the four-digit PIN. Other players enter it under UNIRSE A PARTIDA PRIVADA.
4. Once everyone is connected, the host starts or loads the cooperative game.
Rooms allow a maximum of four players. Players do not need developer accounts or private development credentials.
Troubleshooting
- MULTIJUGADOR does not appear: run the installer again and confirm you selected the folder containing the executable you actually launch.
- No public rooms appear: everyone must use this version, select EOS, and have a public room open. Private rooms are accessed using their PIN.
- EOS helper or configuration missing: extract the complete ZIP and reinstall.
- Checking the installation: run this command from the extracted package folder, replacing the example game path:powershell -NoProfile -ExecutionPolicy Bypass -File .\Instalar-SH2Coop.ps1 -GameDirectory "D:\SH 2" -VerifyOnly
See TEST-RESULTS.md for the tests performed and remaining limitations.
<img width="460" height="107" alt="image" src="https://github.com/user-attachments/assets/392bf195-5601-40fb-ba1e-67df856cde44" />
<img width="456" height="176" alt="image" src="https://github.com/user-attachments/assets/fc17a4d4-4eaa-4c5d-b1be-91a1dfb7bde9" />
Requires Enhanced Edition
(Codex’s collaboration was used to carry out this project.)
