# Lost / Stolen Device Response Solution Pack

## Release Information

- Solution Pack Version: 1.0.0
- Minimum Compatible FortiSOAR™ Version: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

*Lost / Stolen Device Response Solution Pack* is designed to provide a set of investigation playbooks to respond to lost/stolen devices information provided by the end-user through email. These emails are typically reported by employees in the organization (sent to a SOC common email inbox).

Configure Email ingestion using Connectors such as Microsoft Exchange. Ingestion process creates an alert of type 'Lost/Stolen', and then triggers the response workflow.

Refer to Simulation Scenarion - "Device Reported as Lost or Stolen" to experience the use case without any email configuration.

### Usage

This Solution Pack ships with following simulation scenarios. [Refer](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to Simulate Scenario documentation to undersand how to Simulate and Reset Scenario.

#### 1. Scenario - Device Reported as Lost or Stolen

The scenario generates a demo alert of Type 'Lost / Stolen'.
Goto generated alert and observe the following:

- Reported Email contains Device information like Device Owner, Device Type, Device Serial Number etc.
- Reported Information (sender, email message) is presented for analyzing the case.

**Investigate Lost or Stolen Device Response** : Launch "Investigate Lost or Stolen Device Response" Playbook and observe various investigation activities such as

- Asset details from ServiceNow
- Created Asset in FortiSOAR
- User and Manager details from Active Directory
- Sent the Device confirmation detail to the End User and his/her Manager
- Isolated lost/stolen device using Fortinet FortiEDR

## Prerequisites

|**Solution Pack Name**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents

1. Record Set(s)
    - Scenario: Device Reported as Lost or Stolen
2. Connector(s)
    |**SN**|**Connector Name**|
    | :- | :- |
    |1|Microsoft Active Directory|
    |2|Fortinet FortiEDR|
    |3|ServiceNow|

     **Warning:** After deployment, this Solution Pack installs or upgrades the stated list of connectors.
3. Playbook Collection(s)
    - 02 - Use Case - Lost or Stolen Device Response (2):

    |**SN**|**Playbook Name**|**Description**|
    | :- | :- | :- |
    |1|Investigate Lost or Stolen Device Response|Investigates lost or stolen devices using ServiceNow and Active Directory.|
    |2|Generate Alert - Device Lost or Stolen|Generate a device lost/stolen email alert|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
