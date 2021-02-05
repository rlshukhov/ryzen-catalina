# Lane's OpenCore config
#### OpenCore version 0.6.5
#### macOS version Catalina 10.15.7


- [System configuration](#system-configuration)
    - [General](#general)
    - [Other](#other)
- [What is worked](#what-is-worked)
    - [Hardware](#hardware)
    - [Software](#software)
- [What is broken](#what-is-broken)
    - [Hardware](#hardware-1)
    - [Software](#software-1)
- [Installation](#installation)
- [Helpful links](#helpful-links)


## System configuration
### General
- CPU
    - AMD Ryzen R5 3600XT
- Motherboard
    - AsRock B450 Pro4 (ATX)
- RAM
    - HyperX Fury DDR4 3200Mhz 32Gb (2x16Gb)
- GPU
    - Sapphire PULSE RX 560D OC (for hackintosh)
    - GIGABYTE GeForce RTX 2080 SUPER (for Windows)
- PCIs
    - Fenvi FV-T919 (Bluetooth + Wi-Fi card)
### Other
- Cooling
    - CPU DeepCool Gammaxx 300 Fury
    - Case DeepCool GS120 (x3 pcs.)
- Case
    - AeroCool Cylon ATX
- SSD
    - 1Tb M2 Crucial CT1000P1SSD8
- Monitor
    - Samsung C27JG50QQI 2k 144Hz Curved
- Power supply
    - Chieftec SILICON SLC-650C 650W Bronze
- Peripheral
    - Keyboard Motospeed CK108
    - Apple Magic Trackpad 2


## What is worked
### Hardware
- GPU's acceleration with RX 560D
- USB ports (2.0 and 3.0)
- Built-in ethernet (but in this config MB's ethernet is disabled)
- Wi-Fi and Bluetooth
- Motherboard's audio
- External USB mic
- AirPods Pro

### Software
- XCode, iOS Simulator, Safari and other Apple software
- Apple ID (iCloud, iMessage, Apple Music, App Store, iCloud Drive and other)
- Ecosystem: handoff, cloud clipboard, unlock Mac with Apple Watch and other
- Adobe software: Photoshop 2020 (with fix, see below)
- Oracle VirtualBox (and docker-machine too)
- JetBrains IDEs: Android Studio, PHPStorm and other
- iStat Menu
- Microsoft Apps: Office (Word, Excel), Edge, RD Client
- other...


## What is broken
### Hardware
- Nvidia GPU
- A built-in ethernet disabled specially
- CPU temperature monitoring

### Software
- iCloud keychain sync
- Hypervisor Framework and Docker Engine (but you can use `docker` with `docker-machine`)
- Virtualization acceleration with Intel HAXM (Android emulator)
    - You can use ARM images to run an android emulator, but this is slowly


## Installation 
- Read [OpenCore installation guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Fix iServices](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html)
- Note: **in this config serials and mac-address in empty**

## Helpful links
- Docker on AMD hackintosh: [one](https://gist.github.com/slykar/e92732be9bf81a71e08068245656d70e), [two](https://evgeni.blog/hackintosh/docker-amd-ryzen)
- [Fix Adobe software](https://gist.github.com/naveenkrdy/26760ac5135deed6d0bb8902f6ceb6bd)

