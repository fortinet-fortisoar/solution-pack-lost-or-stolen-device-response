| [Home](https://github.com/fortinet-fortisoar/solution-pack-lost-or-stolen-device-response
/blob/develop/README.md) | 
|--------------------------------------------|

# Usage

Refer to [Simulate Scenario documentation](https://github.com/fortinet-fortisoar/solution-pack-soc-simulator/blob/develop/docs/solution-pack-guide.md) to understand how to simulate and reset scenarios. 
 
To understand the process FortiSOAR follows to respond to phishing emails, we have included a scenario &mdash; **Device Reported as Lost or Stolen** with this solution pack. Refer to the section **Device Reported as Lost or Stolen** to understand how this solution pack's automation addresses your needs. 

## Device Reported as Lost or Stolen**

This scenario generates an example alert of type **Lost / Stolen** in FortiSOAR's **Alerts** module.

Navigate to the example alert and observe the following:

- Reported Email contains following device information:
    - Device Owner
    - Device Type
    - Device Serial Number
- Following reported information is presented for analyzing the case:
    - sender
    - email message

## Investigate Lost or Stolen Device Response

Select the alert and launch the playbook **Investigate Lost or Stolen Device Response** to perform following automated tasks:

- Fetch asset details from ServiceNow
- Create asset in FortiSOAR
- Fetch user and manager details from Active Directory
- Send the device confirmation detail to end users and their managers
- Isolate lost/stolen device using Fortinet FortiEDR

