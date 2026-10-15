# Changelog

All notable changes to this project will be documented in this file.

## [1.4] - 2026-10-15

### Added
- Added "Siemens MAG8000" meter type: full AT command config (COMMAND1-4, DATACUT, CLOCKLOG, PARITY) reading Flow, Forward+Reverse Total, Alarm, Battery.
- Added shorter log-interval options: 1m, 2m, 3m, 5m, 6m.
- Added NTP server for Malaysia (my.pool.ntp.org).

### Changed
- MAG8000 MQTT topics now get a "MAG_" prefix to distinguish them from other meter types; config read-back now correctly recognizes MAG8000's 5-segment topic format.
- AT+5VT changed from 1000 to 4000.
- Debug file/debug log: "AT+" is now replaced with "Vilog_" when writing to file and displaying, to mask the raw AT commands.

## [1.3] - 2026-07-10

### Added
- Added debug file feature: allows writing debug logs/data to a file to support monitoring and troubleshooting.

### Changed
- Updated the UI to align with the VilogDLC app's interface.
