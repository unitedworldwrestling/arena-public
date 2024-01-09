# Arena

**Arena is an On Venue Results Management System for Combat Sports.**

It is has been developed and is actively maintained by the **[United World Wrestling IT Department](http://uww.io)**.

**[United World Wrestling](https://unitedworldwrestling.org)** uses **Arena** to manage its Officials International Competitions.

## Install

- [Download VirtualBox](https://www.virtualbox.org/wiki/Downloads) and Install it
- [Download Arena VM (1.5.85)](https://we.tl/t-KX03zM1fli) [MD5: 2024f71cf413233eb41d28ad5157aab2]
    - Legacy [Arena VM (1.5.83)](https://we.tl/t-OCRfO6E4u1) [MD5: bb42f64c94803840cf8dbe0b018530ea]
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
- [UWW IT Webinars - Arena Training Series](https://uww.org/training-education?field_webinar_type_target_id=2024&field_date_range_time_value=All)
    - [Arena Training Series - Overview and Install](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E01/HLS/ArenaTrainingS01E01.m3u8&thumbnail=)
    - [Arena Training Series - Running events](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E02/HLS/ArenaTrainingS01E02.m3u8&thumbnail=)
    - [Arena Training Series - Arena advanced feature - Part I.](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E03/HLS/ArenaTrainingS01E03.m3u8&thumbnail=)
    - [Arena Training Series - Arena advanced feature - Part II.](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E04/HLS/ArenaTrainingS01E04.m3u8&thumbnail=)
    - [Arena Training Series - Companion applications](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E05/HLS/ArenaTrainingS01E05.m3u8&thumbnail=)
    - [Arena Training Series - REST API Interface](https://video.uww.org/embed/bc_external?src=https://d2gmw1lx5tges0.cloudfront.net/assets/ArenaTrainingS01E06/HLS/ArenaTrainingS01E06.m3u8&thumbnail=)

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
- [Version 1.2.38.16](https://github.com/unitedworldwrestling/arena-public/raw/releases/uwwtiming/UWWtimingSetup_1.2.38.16.msi) (14-Mar-2023) - Starting from this version, it requires Arena v1.5.85+
- [Version 1.2.39.27](https://github.com/unitedworldwrestling/arena-public/raw/releases/uwwtiming/UWWtimingSetup_1.2.39.27.msi) (13-Oct-2023)
- [Some previous versions are available here](https://github.com/unitedworldwrestling/arena-public/tree/releases/uwwtiming) - For Arena version earlier than 1.5.85 

#### Usage
Watch the UWW IT Webinars - Arena Training Series - Companion applications video for details.

### Live Graphics Application [Windows Only]

- [Download](https://we.tl/t-XWilLiRzdU) (If this link does not work, visit https://github.com/unitedworldwrestling/arena-public/blob/releases/lgtv/download.link)
- [Documentation](https://github.com/unitedworldwrestling/arena-public/tree/releases/lgtv)

## API

Arena has a built-in Rest API which allows you to extend the main scope of the project.
[API Documentation](http://arena.unitedworldwrestling.org/api/doc)
