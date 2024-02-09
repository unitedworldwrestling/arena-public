Changelog
-------------
1.2.39.42 (09-Feb-2024)
 - Allow to change points during challenge
 - Shows Verbal Warning & Passivity in score timeline
 - Fix Beach Wrestling tie criteria

1.2.39.27 (13-Oct-2023)
 - Fixes to Kazakh mode
 - Fix Start/Stop button is disabled in Desktop mode

1.2.39.22 (11-Aug-2023)
 - New: Add flag for AIN
 - Update: Disable time start/stop button at reaching the Max number of cautions 
 - Update: Change the color of the timer at round ends  

1.2.39.9 (30-May-2023)
 - Fix: Some user is experiencing crash at startup. These errors are being logged now and application can be launched.
 - Update: Add the Event ID and Event name to the "mch" UDP message

1.2.39.4 (05-Apr-2023)
 - New: Submit challenge information to Arena (requires Arena 1.5.86 or later)
 - Update: Beach Wrestling – underline winner in case of a tie 0:0
 - Update: Add transparent white frame around flags on Waiting Screen
 - Update: Updated UI design
 - Update: Validate ArenaURL format on Setup screen
 - Fix: Missing Advantage button in Tablet mode
 - Fix: Referee numbers are not always shown on Waiting Screen
 - Fix: some minor fixes

1.2.38.16 (14-Mar-2023)
 - New: Logfile to store application logs for troubleshooting (%LOCALAPPDATA%\UnitedWorldWrestling\Log)
 - Update: Improve flags readability on the Waiting screen
 - Fix: Application may crash at launch time
 - Fix: Showing matches from weight categories marked as invisible to public in Arena

1.2.38.4 (13-Feb-2023):
Arena 1.5.85 or later requires this version as minimal. Earlier versions of UWWtiming CANNOT work with the new versions of Arena!
 - Compatible with the new authentication method of Arena 1.5.85+
 - New: Autodiscover Arena credentials (Setup window)

1.2.37.16 (07-Dec-2022):
 - New: Ability to select a specific event at Load Matches (Available Fights) screen and process matches only from that event.
 - New: Ability to cancel challenge popup. Available options are Won/Lost and cancel.
 - Fix: “Arena is not available” popup is shown multiple times if Arena is not available. From now, it’s shown only once 

1.2.37.5 (28-Oct-2022):
 - Fix: In some cases Arena Start List shows the same match info about the running match above multiple mats

1.2.37.2 (14-Oct-2022):
 - Support up to 26 mats
 - UDP message “mch” is expanded with weight category id

1.2.36.8 (02-Aug-2022):
- Fix: High CPU utilization detected during application usage
- Fix: Adjusting Activity timer does not work properly in countdown mode

1.2.36 (27-Jun-2022):
 - Improved network outage management
 - Support up to 10 mats

1.2.35 (27-Mar-2022):
 - Setup panel has new option: Scoreboard margin. This allows to set a border around the TV screen scoreboard where the TV does not support fit to screen in full screen mode
 - Fix: Cautions don't get updated when matches flips between styles

1.2.34.5 (15-Feb-2022):
 - Tablet mode shows scores technical points in both rounds
 - Intorucing Leg Fouls
 - Further UI imrpvements for Tablet mode

1.2.33.35 (7-Nov-2021):
 - Further UI improvements for tablet mode (aka Alternate UI)
 - Fix: Next match screen does not load automatically

1.2.33.13 (29-Oct-2021):
 - UI fixes for tablet mode
 - Network timeout adjustment

1.2.33.0 (27-Oct-2021):
 - Sending cautions along with technical points to Arena

1.2.32.23 (4-Oct-2021):
 - Update on Bahrain flag (BRN)
 - Logfiles are stored under %LOCALAPPDATA%\UWWTiming folder

1.2.32.18 (28-Sep-2021):
 - Fix Russian flag (RWF)

1.2.32.15 (27-Sep-2021):
 - New flag: ROC is added
 - Update: flag rendering module is ugpraded

1.2.32.12 (21-Sep-2021):
 - New: Beach Wrestling - show weight of the wrestlers (if recorded in Arena) on End Of Match screen
 - Fix: UI fixes for Beach Wrestling fights
 - Fix: AutoUpdate closes the application automatically
 - Some updates on Mercure server communication

1.2.32.1 (1-Sep-2021):
- New: new matches are refreshed in the background
- New: Custom timer settings are retained
- Improvements on Network packets
- Fix: Rest time is not recalculated for new matches
- Fix: UI fixes

1.2.31.1 (11-Feb-2021):
 - Support for Kazakh Kuresi scoreboard type
 - Some UI fixes in tablet mode

1.2.30.16 (01-Feb-2021):
 - Fix: Can't send match results to Arena in some cases

1.2.30.13 (26-Jan-2021):
 - New: Auto Updater module
 - Fix: Unable to load matches from Arena 1.5.70, Time is displayed in invalid format, Period does not end

1.2.30 (8-Dec-2020):
 - New: Verbal Warning button
 - New: Overtime support (requires Arena support)
 - New: Dynamic number of cautions (requires Arena support)
 - New: Autoupdate
 - Fix: Preserve settings across upgrades
 
1.2.29.22 (20-Apr-2020):
 - Using new installer

1.2.29.17 (20-Apr-2020):
 - Redesigned End of Match buttons (generated according to the weight category Victory types)
 - Beach Wrestling has "Bleeding" time instead of "Injury"
 - Exposing match details via SocketIO protocol 
