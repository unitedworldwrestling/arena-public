# Arena

**Arena is an On Venue Results Management System for Combat Sports.**

It is has been developed and is actively maintained by the **[United World Wrestling IT Department](http://uww.io)**.

**[United World Wrestling](https://unitedworldwrestling.org)** uses **Arena** to manage its Officials International Competitions.

## Install

- [Download VirtualBox](https://www.virtualbox.org/wiki/Downloads) and Install it
- [Download Arena VM (1.5.76)](https://we.tl/t-zIFQfJSnGi) [MD5: c0a7c9744a4b26560198fe68ba9776d8]
    - (Legacy [Arena VM (1.5.74.1)](https://we.tl/t-BPiEKwEXGo) [MD5: e2b1e13ee5dda5efef424ff649ed80bc])
- Open VirtualBox
- Go to File > Import Appliance > Select the Arena VM you just downloaded
- Continue with the default settings
- Double-click on the newly created VM to start it (You can then reduce this Window)
- Go to [http://localhost:8080](http://localhost:8080/)

## Upgrade

If a new version is available you wil see an "Upgrade" button on the top right corner, just click and wait.

**Known issue:** 

You may receive "ERROR: Error installing bundler" message during upgrade. To fix the error follow these steps:
- Download the arena_upgrade executable for the Operating System where Arena is running (Find them in the [Wiki](https://github.com/unitedworldwrestling/arena-public/wiki/How-to-use-arena_upgrade-application))
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
- [UWW IT Webinars - Arena Training Series](https://uww.org/webinars?field_webinar_type_target_id=2024&field_datetime_value=All)

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

The application offers an automatic update if a new version is available. Please read the Changelog displayed by the Autoupdater to learn about the changes
- [Version 1.2.33.0](https://github.com/unitedworldwrestling/arena-public/raw/releases/uwwtiming/UWWtimingSetup_1.2.33.0.msi) (27-Oct-2021)
- [Old versions are available here](https://github.com/unitedworldwrestling/arena-public/tree/releases/uwwtiming)

#### Usage
Watch the UWW IT Webinars - Arena Training Series - Companion applications video for details.

### Live Graphics Application [Windows Only]

- [Download](https://github.com/unitedworldwrestling/arena-public/tree/releases/lgtv)
- [Documentation](https://github.com/unitedworldwrestling/arena-public/tree/releases/lgtv)

## API

Arena has a built-in Rest API which allows you to extend the main scope of the project.
[API Documentation](http://arena.unitedworldwrestling.org/api/doc)
