# Arena

**Arena is an On Venue Results Management System for Combat Sports.**

It is has been developed and is actively maintained by the **[United World Wrestling IT Department](http://uww.io)**.

**[United World Wrestling](https://unitedworldwrestling.org)** uses **Arena** to manage its Officials International Competitions.

## Install

- [Download VirtualBox](https://www.virtualbox.org/wiki/Downloads) and Install it
- [Download Arena VM (v1.5.70)](https://we.tl/t-xlwwA0Lla9) [MD5: 712e7f1b7acfa32386716224df6245c0]
    - (Legacy [Arena VM v1.5.43](https://we.tl/t-aLRG4nx4aC)) [MD5: 9181d241ff5ae30cc3299bd2df481d6b]
- Open VirtualBox
- Go to File > Import Appliance > Select the Arena VM you just downloaded
- Continue with the default settings
- Double-click on the newly created VM to start it (You can then reduce this Window)
- Go to [http://localhost:8080](http://localhost:8080/)

## Upgrade

If a new version is available you wil see an "Upgrade" button on the top right corner, just click and wait.

**Known issue:** 

You may receive "ERROR: Error installing bundler" message during upgrade. To fix the error follow these steps:
- Download the arena_upgrade executable for the Operating System where Arena is running ([Windows 64bit](https://we.tl/t-VmvUfSvy59), [Windows 32bit](https://we.tl/t-uEbXF1tjID), [macOS](https://we.tl/t-rdW30UTKEd))
- Make sure Arena is running and accessible via [http://localhost:8080](http://localhost:8080/)
- Open Command Prompt (Windows) or Terminal (macOS)
- Run arena_upgrade from its download folder (on macOS, you may have to grant execute permission to the command by "chmod +x arena_upgrade_osx")
- Wait until the upgrade completes

## Reporting problems

Support requests, bugs can be reported on the [Github issues tracker](https://github.com/unitedworldwrestling/arena-public/issues).

## Features

- Individual / Team competitions
- Single elimination / Double elimination / Round-Robin Tournaments
- Custom Weight Categories
- Sessions Optimization
- Rest Time Management
- Results Checker
- Score Sheets printing
- Rankings
- PDF Reports
- Referees assignment
- On-Screen display
- Offline access
- Centralize DataBase Synchronization
- Web-Formated results
- API

## Usage

### Webinars
- [UWW IT Webinars - Arena Training Series](https://unitedworldwrestling.org/webinars?field_webinar_type_target_id=2024)

### Frontend
- [http://localhost:8080](http://localhost:8080)

### Backend

- [http://localhost:8080/bracket](http://localhost:8080/bracket)

### On Venue Features

- [http://localhost:8080/onvenue](http://localhost:8080/onvenue)

### Wrestling Competition Workflow

- Add event
- Add Weight Categories
- Add Athletes
- Draw Weight Categories
- Create Matches
- Print Score Sheets
- Check Results
- Print Reports

## External Applications

Arena comes with a Score Board & Live Graphics application.

### Score Board [Windows Only]

Be careful to download the version corresponding to your version of Arena.
- [Version 1.2.31.1](https://github.com/unitedworldwrestling/arena-public/raw/releases/uwwtiming/UWWtimingSetup_1.2.31.1.msi) (11-Feb-2021)

#### Usage
The following steps should be executed on the computer running the Score Board / Weigh-In.

- Install with the default settings
- Open UWW_configurator.exe
- Fill the "Server URL" with the Arena IP: ````192.168.1.1:8080```` (replace the IP address with the server IP)
- Select the Mat related to this Score Board (Mat A by default)
- Save
- Open UWW_timing.exe

### Live Graphics Application [Windows Only]

- [Download](https://we.tl/t-GysVJKuk1c)
- [Documentation](https://we.tl/t-AgRGognV6g)

## API

Arena has a built-in Rest API which allows you to extend the main scope of the project.
[API Documentation](http://arena.unitedworldwrestling.org/api/doc)
