# User Manual

## Purpose

IEC60870 101/104 Protocol Test Analyzer is built to support FAT, SAT, and SCADA commissioning work for IEC 60870-5-104 and IEC 60870-5-101 systems.

This tool helps engineers validate point mapping, observe protocol behavior, investigate command mismatch, review SOE and event flow, and identify reliability issues earlier.

## Main Workflow

1. Start the analyzer.
2. Select IEC-104 or IEC-101 connection settings.
3. Connect to the target endpoint.
4. Observe line monitor, values, events, findings, and status history.
5. Run command tests and verify response behavior.
6. Save capture files for replay and reporting.

## Core Panels

### Line Monitor

The line monitor presents protocol activity in a human-readable flow, making it easier to understand actual IEC traffic without reading raw packets only.

![Line Monitor](../assets/images/17-line-monitor.png)

Use this panel to:

- inspect protocol sequence flow
- verify COT and ASDU activity
- see command and response timing
- review event bursts and message direction

### Last Known Values

This panel is used for fast point-to-point cross-check between field and SCADA master.

![Last Known Values](../assets/images/16-last-known-values.png)

Use this panel to verify:

- IOA mapping
- value and quality
- COT behavior
- derived class information
- context and timestamp consistency

### Findings

The Findings panel highlights observations that may indicate reliability or engineering issues.

![Findings](../assets/images/06-findings-panel.png)

Typical findings include:

- command activation without confirmation
- traffic after disconnect request
- suspicious event sequence behavior
- recommendations to improve reliability

### Status History

Status History provides a useful audit trail of connection lifecycle, command actions, and important runtime events.

![Status History](../assets/images/23-status-history.png)

Use this for:

- FAT and SAT evidence
- troubleshooting session behavior
- reviewing connect, disconnect, and command actions

## Command Testing

The analyzer supports practical command testing workflows from one interface.

![Command Function Selector](../assets/images/11-command-function-selector.png)

Available command-oriented views include:

- General Interrogation
- Time Synchronization
- Single Command
- Double Command
- Setpoint Command

### General Interrogation

![General Interrogation](../assets/images/14-general-interrogation.png)

### Time Synchronization

![Time Sync Command](../assets/images/24-time-sync-command.png)

### Single Command

![Single Command](../assets/images/21-single-command.png)

### Double Command

![Double Command](../assets/images/12-double-command.png)

### Setpoint Command

![Setpoint Command](../assets/images/20-setpoint-command.png)

## Utility Features

### IOA Converter

The structured IOA converter helps engineers translate between structured IOA components and flat IOA values.

![IOA Converter](../assets/images/15-ioa-converter.png)

This is useful when checking RTU, gateway, and SCADA engineering data.

### Protocol Context

![Protocol Context](../assets/images/18-protocol-context-panel.png)

Use this panel to review protocol-related context information while testing.

### Glossary

![Glossary](../assets/images/01-glossary.png)

The glossary provides quick interpretation support for protocol terms and objects.

## Event and Analysis Views

### Event Log Panel

![Event Log Panel](../assets/images/13-event-log-panel.png)

### SOE Event Log Panel

![SOE Event Log Panel](../assets/images/22-soe-event-log-panel.png)

### SCADA Event Log Panel

![SCADA Event Log Panel](../assets/images/19-scada-event-logs-panel.png)

These views help engineers compare field events with SCADA-side interpretation and timestamp behavior.

## Connection Setup

### IEC-104

![IEC-104 Connection Setup](../assets/images/01-connection-setup-iec104.png)

### IEC-101

![IEC-101 Connection Setup](../assets/images/02-connection-setup-iec101.png)

## Capture and Replay

The analyzer supports capture save and replay workflows for post-test analysis, investigation, and report evidence.

![Save Capture](../assets/images/09-save-capture.png)
![Open Replay](../assets/images/10-open-replay.png)

## Recommended Field Use

Use this tool when you need to investigate:

- command mismatch between SCADA and RTU or gateway
- Class 1 and Class 2 assignment issues
- Type ID mismatch and interpretation problems
- value or quality mismatch
- SOE timestamp inconsistency
- worst-case traffic behavior under measurement burst
