| [Home](https://github.com/fortinet-fortisoar/solution-pack-lost-or-stolen-device-response
/blob/develop/README.md) | 
|--------------------------------------------|

# Installation

1. To install a solution pack, click **Content Hub** > **Discover**.    
2. From the list of solution pack that appears, search for and select **Lost or Stolen Device Response**.
3. Click the **Lost or Stolen Device Response** solution pack card.    
4. Click the **Install** button on the bottom to begin installation. 

## Prerequisites

| Solution Pack Name | Purpose                                                 |
|:-------------------|:--------------------------------------------------------|
| SOAR Framework     | Required for Incident Response modules                   |
| SOC Simulator      | Required for Scenario Module and SOC Simulator connector |

# Configuration

For optimal performance of **Lost or Stolen Device Response** solution pack, you can install and configure: 
- An email ingestion process to periodically read email from a designated inbox and convert them into alerts in FortiSOAR 
    - To configure and use MS Exchange for email ingestion, refer to [Configuring Exchange Connector](https://docs.fortinet.com/document/fortisoar/3.4.0/exchange/1/exchange-v3-4-0#Configuring_the_connector)
- An asset management system to track the issued devices
    - To configure and use ServiceNow as an asset management system, refer to [Configuring ServiceNow Connector](https://docs.fortinet.com/document/fortisoar/3.1.0/servicenow/134/servicenow-v3-1-0#Configure_Data_Ingestion)
- An EDR solution to isolate the device
    - To configure and use Fortinet's FortiEDR as an EDR solution, refer to [Configuring Fortinet FortiEDR Connector](https://docs.fortinet.com/document/fortisoar/1.3.0/fortinet-fortiedr/161/fortinet-fortiedr-v1-3-0#Configure_Data_Ingestion)