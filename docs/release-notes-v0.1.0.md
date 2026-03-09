# v0.1.0 - Free IEC60870 FAT/SAT Analyzer Public Release

First public binary release of IEC60870 101/104 Protocol Test Analyzer.

This release introduces an internally developed diagnostic support platform intended to improve IEC-101 and IEC-104 verification workflow during FAT, SAT, commissioning, troubleshooting, and product readiness activities.

## Why This Release Matters

- Supports a more transparent and repeatable verification workflow
- Helps reduce troubleshooting iteration through better protocol visibility
- Improves technical evidence quality for FAT, SAT, and issue clarification
- Supports earlier detection of data class, IOA mapping, and command behavior issues
- Extends value beyond project execution into homologation or certification readiness support

## Highlights

- IEC-104 and IEC-101 protocol test workflow support
- Human-readable line monitor for protocol flow analysis
- Last known value viewer for IOA, value, quality, COT, class, and timestamp cross-check
- Internal event logs, SOE-oriented analysis, and status history
- Findings panel for reliability improvement insight
- Command panel for testing GI, time sync, single, double, and setpoint command scenarios
- Capture save and replay workflow for investigation and reporting
- Includes `IecSlaveSimulator.exe` helper tool

## Practical Value

The platform is intended to help engineering teams:

- accelerate FAT and SAT troubleshooting cycles
- reduce repeated point-to-point rework
- improve confidence before handover and energization
- support certification readiness where Data Class and ACD behavior must be clarified

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
- The platform is intended as a supporting diagnostic aid and complements existing engineering checks.
- IEC-101 capability is available and may continue evolving in future releases.
