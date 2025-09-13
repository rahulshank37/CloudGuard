# CloudGuard
Deployed Azure Sentinel with a Logic App to automate security monitoring and alerting. Configured analytics rules to detect failed logins, privileged identity assignments, and sign-ins from outside the U.S. The Logic App triggers notifications and workflows, enabling faster visibility and response.


# Sentinel-LogicApp-Security-Monitoring

## Project Overview
This project demonstrates the deployment of Azure Sentinel integrated with a Logic App to automate security monitoring and alerting. The solution enhances visibility into Azure activity by detecting and responding to key security events.

## Features
- Azure Sentinel Integration: Centralized security monitoring and log management.  
- Logic App Automation: Triggers workflows and notifications on security events.  
- Custom Analytics Rules:  
  - Detects failed login attempts  
  - Alerts on privileged identity assignments  
  - Flags sign-ins originating outside the U.S. region  

## Architecture
1. Azure Sentinel connected to Log Analytics Workspace  
2. Custom Analytics Rules configured to detect suspicious events  
3. Logic App triggered by Sentinel incidents  
4. Notification Workflow sends alerts to designated recipients  

## Deployment Steps
1. Deploy Azure Sentinel and connect it to your Log Analytics Workspace  
2. Configure Analytics Rules for:  
   - Failed sign-in attempts  
   - Privileged identity assignments  
   - Non-U.S. sign-ins  
3. Deploy the Logic App and connect it with Sentinel  
4. Configure Logic App actions to send alerts (e.g., email, Teams, or other connectors)  
5. Test by simulating failed logins or non-U.S. sign-ins  

## Benefits
- Real-time detection of suspicious sign-ins  
- Automated alerting for faster incident response  
- Improved security visibility across Azure environments  

## Notes
- Designed for testing and demonstration purposes  
- Extendable for enterprise use by adding more rules (e.g., impossible travel, role changes, risky sign-ins)  
