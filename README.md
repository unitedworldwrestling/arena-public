# Arena

**Arena is an On Venue Results Management System for Combat Sports.**

It is has been developed and is actively maintained by the **[United World Wrestling IT Department](http://uww.io)**.

**[United World Wrestling](https://unitedworldwrestling.org)** uses **Arena** to manage its Officials International Competitions.

## Install
1. Download and install Docker Desktop https://docs.docker.com/desktop/
2. Copy [docker-compose.yaml](https://github.com/unitedworldwrestling/arena-public/blob/master/Resources/docker-compose.yaml) into a folder (You must remember this folder location, or use the commands from the "Upgrading to a newer version" section below!!!)
    - On Windows, it's recommended to use WSL2 (Ubuntu)
3. Run `docker compose pull` command from the **same** directory of docker-compose.yaml
    - If you receive "Rate exceeded" error, either Sign in to Docker Desktop, or try with this command 
        - PowerShell: `$env:COMPOSE_PARALLEL_LIMIT='1'; docker compose pull; Remove-Item Env:COMPOSE_PARALLEL_LIMIT`
        - Linux/macOS shell: `COMPOSE_PARALLEL_LIMIT=1 docker compose pull`
5. Run `docker compose up -d` to get Arena running

## Upgrade

If a new version is available you wil see an "Upgrade" button at the top right corner under the admin interface (/bracket)
> [!Important]
> You must run docker commands from a Terminal application (Poweshell on Windows, or shell on Linux/macOS) and from the directory where you originally downloaded `docker-compose.yaml` and installed Arena first time.
> If you forgot the directory where this file was downloaded, use the following command to identify:
> 
> The last parameter of the following commands is `arena-php-fpm-1` (`<first part>-<second part>`)
> ![image](https://github.com/user-attachments/assets/bb0d96ec-7721-465a-bcb8-29b50f92e2e4)
> 
> Poweshell:
> ```powershell
>  docker inspect --format='{{index (index .Config.Labels \"com.docker.compose.project.working_dir\")}}' arena-php-fpm-1
> ```
>
> Linux/macOS shell:
> ```bash
>  docker inspect --format='{{index (index .Config.Labels "com.docker.compose.project.working_dir")}}' arena-php-fpm-1
> ```

So first, make sure you have the latest `docker-compose.yaml` file. You will get notified by Arena if your [docker-compose.yaml](https://github.com/unitedworldwrestling/arena-public/blob/master/Resources/docker-compose.yaml) file version is not the most recent. Download the latest version and update your existing file.

To upgrade Arena, it's recommended to run `docker compose pull` command from the `docker-compose.yaml` file's directory. You may have to Sign In to Docker Desktop or set `COMPOSE_PARALLEL_LIMIT` variable (as described under Install section) in case of "Rate exceeded" error message during `pull`.

> [!Important]
> After the `pull` command, the containers MUST BE restarted with `docker compose up -d` command.

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
- [Available Versions can downloaded from here](https://github.com/unitedworldwrestling/arena-public/tree/releases/uwwtiming) (always download the latest version!)

#### Usage
Watch the UWW IT Webinars - Arena Training Series - Companion applications video for details.

### Live Graphics Application [Windows Only]

- [Download](https://we.tl/t-KQDJvizNRH) (If this link does not work, check [the current one](https://github.com/unitedworldwrestling/arena-public/blob/releases/lgtv/download.link)
- [Documentation](https://github.com/unitedworldwrestling/arena-public/tree/releases/lgtv)

## API

Arena has a built-in Rest API which allows you to extend the main scope of the project.
[API Documentation](http://arena.unitedworldwrestling.org/api/doc)
