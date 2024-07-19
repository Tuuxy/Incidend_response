# Detecting the Cyber Incident 

## Prevention is ideal, but detection is a must

Assume the adversary is already inside our network.
We can't prevent all attacks, but when they are inside that is when we need to detect them. 

## Detection Sources

- Cloud: Cloud Access Security Brokers (CASB), Multifactor Authentication (MFA), SaaS Logs, Usage and Data Transfer Logs, AWS/Azure Logs,...

- User Activity: Access Attempts, Login Information, MFA Usage, User Entity Behavior Analytics (UEBA), Software Installation, Hardware installation,...

- Applications: Database Access and Changes, Application Privilege Escalation, Sensitive Data Access, Modification of Security Controls, System Notification Messages, Security Events,...

- Mobile Devices: Mobile Device Management (MDM) Logs, App Installation, Containerization Logs, Location Information, Attemps to Circumvent Security Controls,...

- User Complaints: Complaints from HR, Reports from Users, Complaints from Management,...

- Desktops/Laptops: Endpoint Detection & Response (EDR) Tools, Host Intrusion Detection, Process Execution, Registry Changes, Evidence of Persistence,...

- Servers & Virtualized Infrastructure: Host Intrusion Detection, Virtualization Management, SCCM/SCOM Alerts, EDR Alerts,...

- Sensors: Network Taps, EINSTEIN,...

- Network Traffic: Intrusion Detection/Prevention, Firewalls, Sandbox Devices, Proxies, DNS/DHCP, TLS Decryption, Router Tables, Packet Capture,...

## Detect and Analyze Process:

Alert => Triage => Declare an Incident => Investigation 

## SIEM

One of the first tool you should consider implementing if you don't have any SIEM yet.

- Correlation and aggregation of logs from a variety of sources
- Be extremely careful of time and time zones. Always utilize UTC when possible
- Use checklists to ensure data feeds, dashboards and alerts are working daily 
- Have someone "own" the SIEM and maintain and tune it

## Event and Incident Tracking

- Incidents and Events
- Sources of alerts - what is your cost per alert and false positive rate? 
- Users and systems involved
- IP addresses
- Commentary and workflow for incident responders
- Notifications and assignment of actions

https://getscot.sandia.gov

## Be Careful of Too Much Noise

Too many alerts and data sources cause:

- Alert fatigue
- Poor prioritization/Loss of focus
- Inefficient systems/Engineering problems

## Security Analytics

- Descriptive : What happened ? SIEM IDS Threat Intel

- Diagnostic : Why did it happen ? Network Traffic Analysis UEBA

- Predictive : What will happen ? Fraud Detection

- Prescriptive : What should I do ? Security Orchestration, Automation & Response (SOAR) 

## Technical Approaches for Anomaly Detection

- Rule-Based : 
        
        - Signatures
        - Threat Intel
        - Statistics

- Historical Analysis :
        
        - Activity Scoring
        - Timeline View
        - Retrospective Analysis

- Machine Learnin :

        - Detection Algorithm
        - (Un)Supervised Learning

## A Range of Analytics Types is Needed

### Known Knowns

- Whitelists
- Correlation Rules
- IP address or URL match on threat intel
- Multiple account failures across x machines in y minutes

### Known Unknowns

- Supervised / Unsupervised Machine Learning (ML) 
- Supervised: Mainly by vendors based on "known bads"
- Unsupervised: AKA Anomaly detection

### Unknown Unknowns

- Deep learning
- Models determine which features to extract
- Humans label data
- Human train models

## SOAR Capabilities

- Ability to integrate with other security solutions
- Multiple "push" or "pull" capabilities
- API customization between security products
- Allow abstraction of tools and doesn't require analysts to be an expert in everything
- Take standard steps automatically
- Ability to make playbooks

## Defining an Incident (refresher)

- Event : Something that happens on information systems (not required to be malicious or requiring action) ex: successful login

- Alert : Something potentially actionnable. ex: notification of malware on a device

- Incident (small i) : Violation of CIA without a business impact

- Incident (capital i) : Violation of CIA with a business impact

- Breach : Loss of specific data that triggers legal obligations above and beyond

## SOC and IR are not the same thing

## Alert Triage Process Example

![[alerttriageprocess.png]]

## Multiple Incidents Triage

- Potential impact to CIA and safety (dam, grid, traffic lights,...)
- Sensitivity of data involved
- Reputational risk
- Regulatory risk
- Criticality of the assets involved

## Develop an ISCM Program

Define ISCM Strategy => Establish ISCM Program => Implement ISCM Program => Analyze Data & Report Findings => Respond to Findings => Review & Update ISCM Strategy & Program

## Define your ISCM Strategt

### Situational Awareness

- Real-time or near real-time awareness of boundary
- Awareness of threats and threat activities

### Security Controls

- ISCM can access all security controls
- Recurring vulnerability scanning
- Inventory control

### Data 

- Collect, correlate, analyze security - related data
- Provide actionable communications of InfoSec status

### Risk 

- Manage info system risk based on risk tolerance
- Configuration / change management

## Steps for Continuous Monitoring (CM)

- Develop a CM policy that provides appropriate authority and is applicable to everyone
- Develop a strategy to test a subset of security controls. Test them for effectiveness and document findings
- Create a robust configuration control and change control process and policy. Ensure all proposed changes are reviewed to determine the security significance
- Determine reporting requirements, audience and format to communicate risk and status of system monitoring
- Conduct remediation actions based upon monitoring activities
- Update all documents as necessary - continuous monitoring also means continuous documentation of changes to risks, threats, vulnerabilities and controls

## Requirements for Security Configuration

- Must have hardware/software inventory - even if it is excel to begin with
- Policy must define how configuration management will be applied to information systems within the framework established by the organization
- Configuring information systems to a secure state (ie, gold image)
- Managing and controlling changes to information systems(ie, CCBs)

## How continuous is continuous ? 

There is no defined rule but you need to make sure you are following the rules that you define.

Example FedRAMP: 

![[fedramp.png]]
## Sample Detection Metrics

(Remember your audience! Above the line vs. below the line)

1. Mean time to detection
2. Ratio of events to alerts
3. Average time to triage
4. Cost per alert
5. False positive rate
6. Vulnerability scanning coverage
7. Malware detection rate


