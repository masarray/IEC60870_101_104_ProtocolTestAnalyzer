# v0.1.0 - Free IEC60870 FAT/SAT Analyzer Public Release

First public binary release of IEC60870 101/104 Protocol Test Analyzer.

Built as a practical free alternative to expensive protocol analyzers, this tool is designed for real FAT, SAT, and SCADA commissioning work on IEC 60870-5-104 and IEC 60870-5-101 systems.

Instead of only showing raw packets, it helps engineers work faster with clearer data views, internal event logs, SOE cross-check support, capture replay, and actionable Findings that highlight communication issues before they become operational problems.

## Why This Release Matters

- Free to try for real project work
- Built for SCADA, substation, and commissioning engineers
- Speeds up point-to-point validation and troubleshooting
- Helps expose command mismatch, class mismatch, Type ID mismatch, and timestamp issues
- Provides better visibility for communication behavior during burst or worst-case traffic conditions

## Highlights

- IEC-104 and IEC-101 protocol test workflow support
- Human-readable line monitor for protocol flow analysis
- Last known value viewer for IOA, value, quality, COT, class, and timestamp cross-check
- Internal event logs, SOE-oriented analysis, and status history
- Findings panel for reliability improvement insight
- Command panel for testing GI, time sync, single, double, and setpoint command scenarios
- Capture save and replay workflow for investigation and reporting
- Includes `IecSlaveSimulator.exe` helper tool

## Best Use Cases

- FAT and SAT point-to-point validation
- Investigating failed or mismatched commands
- Checking Class 1 and Class 2 traffic behavior
- Cross-checking RTU or Gateway data against SCADA master expectations
- Reviewing SOE timestamp consistency between systems
- Creating evidence for troubleshooting, reporting, and vendor discussion

## Included Files

- `IEC-60870-Protocol-Analyzer.exe`
- `IecSlaveSimulator.exe`
- `lib60870.dll`
- `System.IO.Ports.dll`
- `profiles/default-iec104.json`

## Installation

1. Download the release zip.
2. Extract it to a local folder.
3. Run `IEC-60870-Protocol-Analyzer.exe`.
4. Configure IEC-104 or IEC-101 connection settings.
5. Start monitoring, testing, and reviewing Findings.

## Notes

- This repository provides release binaries only.
- IEC-101 capability is available and can continue improving in future releases.
- This tool is intended to help engineers reduce commissioning time, improve visibility, and catch configuration issues earlier.
