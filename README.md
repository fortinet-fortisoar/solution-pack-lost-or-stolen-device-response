# Lost / Stolen Device Response Solution Pack

## Overview
### Introduction
This article describes the  Lost / Stolen Device Response Solution Pack. The solution pack demonstrates the scenarios and use cases around lost/stolen devices based on using the information provided by the end-user through email.

The scenario demonstrates and generates a demo alert for the Alert Type 'Lost / Stolen'.

The use-case deals with containment and investigation procedures once the end-user reports a lost or stolen device through email.
Create FortiSOAR Alert using the email details received from end-user
-	Get Asset details from ServiceNow
-	Create Asset in FortiSOAR
-	Retrieve User and Manager details from Active Directory
-	Send the Device confirmation detail to the End User and his/her Manager
-	Isolate lost/stolen device using Fortinet FortiEDR
-	Send Email to the IT and HR team 
-	Close the Alert in FortiSOAR


### Usage 
More information about usage of Lost / Stolen Device Response Solution Pack [here](https://github.com/fortinet-fortisoar/solution-pack-lost-or-stolen-device-response/blob/develop/docs/solution-pack-guide.md).

## Version Information
- Solution Pack Version: 1.0.0
- FortiSOAR™ Version Tested on: 7.2.0
- Authored By: Fortinet
- Certified: No

## Prerequisites
**Solution Pack Name**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|
|SOC Simulator 1.0.1|Require for Scenario Module and SOC Simulator connector| [Click here](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/README.md)|

## Contents
1. Record Set(s)
    - Scenario: Device Reported as Lost or Stolen
2. Connector(s)
    **SN**|**Connector Name**|
    | :- | :- |
    |1|Microsoft Active Directory|
    |2|Fortinet FortiEDR|
    |3|ServiceNow|

    **Warning:** After deployment, this Solution Pack installs or upgrades the stated list of connectors.
3. Playbook Collection(s)
    - 02 - Use Case - Lost or Stolen Device Response (4): Following is a list of playbooks under “02 - Use Case - Lost or Stolen Device Response” solution pack.

    **SN**|**Playbook Name**|**Description**|
    | :- | :- | :- |
    |1|Investigate Lost or Stolen Device Response|Investigates lost or stolen devices using ServiceNow and Active Directory.|
    |2|Generate Alert - Device Lost or Stolen|Generate a device lost/stolen email alert|

    **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.