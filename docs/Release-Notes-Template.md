# Release Notes Template

Use this template when publishing a new GitHub Release.

## Title

`vX.Y.Z - Short Release Name`

## Summary

Short description of what this release improves for end users.

## Included Files

- `IEC-60870-Protocol-Analyzer.exe`
- `lib60870.dll`
- `System.IO.Ports.dll`
- `profiles/default-iec104.json`
- other bundled tools or profiles if applicable

## Highlights

- Added:
- Improved:
- Fixed:

## Recommended Use Cases

- FAT and SAT point-to-point verification
- command mismatch investigation
- Class 1 and Class 2 traffic validation
- SOE timestamp cross-check between substation and SCADA master
- capture replay for troubleshooting and reporting

## Known Notes

- State any protocol limitations clearly.
- State any environment assumptions clearly.
- State if IEC-101 support is partial or evolving for that release.

## Installation

1. Download the release zip.
2. Extract to a local folder.
3. Run `IEC-60870-Protocol-Analyzer.exe`.

## Feedback

Use GitHub Issues or your internal feedback channel to report problems found during commissioning.
