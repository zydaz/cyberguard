

# CyberGuard — Use Case Diagram

## Overview

This diagram illustrates the interactions between the external actors and CyberGuard.

## Diagram

```mermaid
flowchart LR
    SOC["SOC Analyst"]
    APP["External Application"]

    subgraph CG["CyberGuard"]
        direction TB
        UC01(["UC-01 Authenticate"])
        UC02(["UC-02 View Security Alerts"])
        UC03(["UC-03 Investigate Events"])
        UC04(["UC-04 Manage Alerts"])
        UC05(["UC-05 Submit Security Events"])
    end

    SOC --- UC01
    SOC --- UC02
    SOC --- UC03
    SOC --- UC04

    APP --- UC05
```

## Actors

- **SOC Analyst:** Monitors alerts and investigates suspicious activities.
- **External Application:** Submits security events for analysis.

## Notes

This Mermaid flowchart is a simplified representation
of the system use cases. A formal UML use case
diagram may be added later.
