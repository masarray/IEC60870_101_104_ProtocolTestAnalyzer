# Quick Start

## Purpose

This release package provides an internally developed diagnostic support tool intended to improve IEC-101 and IEC-104 verification workflow during FAT, SAT, commissioning, troubleshooting, and product readiness activities.

## What You Need

- Windows x64 machine
- Extracted release package from GitHub Releases
- Access to IEC-104 endpoint or IEC-101 serial connection
- Point list or FAT/SAT test sheet for validation

## Package Contents

A typical release package should include:

- `IEC-60870-Protocol-Analyzer.exe`
- `lib60870.dll`
- `System.IO.Ports.dll`
- `profiles/default-iec104.json`
- optional helper tools if shipped with the release

## First Run

1. Download the latest release zip from GitHub Releases.
2. Extract the zip to a local folder such as `C:\Tools\IEC60870-Analyzer`.
3. Run `IEC-60870-Protocol-Analyzer.exe`.
4. Open the connection setup dialog.
5. Choose `IEC-104` or `IEC-101`.
6. Enter connection parameters and start monitoring.

## Recommended First Checks

After connection starts, verify:

- values are updating as expected
- IOA mapping matches the point list
- quality values are reasonable
- SOE event timestamps are consistent
- command tests produce expected responses
- Findings panel does not show critical issues

## Recommended Practical Use

Use the platform to support:

- point-to-point mapping verification between RTU or Gateway and master SCADA
- command behavior validation for DO and SBO schemes
- data class and priority behavior checks under heavy traffic or burst conditions
- Type ID, quality, and timestamp consistency review
- capture replay evidence for FAT/SAT, troubleshooting, and reporting
- readiness review before homologation or certification-related testing

## Troubleshooting Basics

### IEC-104 does not connect

- Check IP address and port.
- Check network reachability and firewall.
- Check common address and remote endpoint status.

### IEC-101 does not connect

- Check COM port number.
- Check baud rate, parity, data bits, and stop bits.
- Check link address and serial wiring.

### Data appears but is wrong

- Compare IOA against the point database.
- Check Type ID and Cause of Transmission.
- Verify scaling, quality, class grouping, and timestamp behavior.

## Related Documents

- [README](../README.md)
- [User Manual](User-Manual.md)
- [Release Notes Template](Release-Notes-Template.md)
- [Package Structure](Package-Structure.md)
