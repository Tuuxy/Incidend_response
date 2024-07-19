# Recovering from a Cyber Incident

## Attempt to Determine the Entry Point

- The beachhead is the intrustion point for an organization
- Usually the beachhead attack is fragile and not persistent
- Determine how the attacker gained entry is important to the investigation

## Restoring Systems

- Ensure systems are restored from known good backups
- Ensure IT and Cybersecurity are lockstep during restoration process
- Don't restore the infection!
- Conduct a coordinated restoration while closely monitoring for IOCs
- If in doubt, conduct forensics on backups
- Have config files encrypted and hashed with hashes recorded

## Conducting the Debriefing / Lessons learned

- Consider who should lead the meeting:
        - CIRT lead
        - CISO
        - Another person in the organization good at facilitation
        - Outside consultant

## Debriefing Topics to Discuss

- How and exactly when was the incident first detected ?
- Was the incident properly triaged and categorized ? 
- What roles did everyone play ? 
- Did the plan work ? What should be changed ? 
- Were all the right notifications made ? 
- What would we do differently ?
- What could we do as a team to improve ? 
- What resources could we have used but didn't have ? 
- What went well ? 

## Debriefing Notes 

- Use notes from the debriefing to help guide the after action report (AAR)
- The focus of the AAR is not to place blame or attribution, but to focus on what went well and what needs to improve

## Constructing the AAR

1. Executive summary
2. Participants and IR team members
3. Incident timeline & details
4. Impact assessment
5. Root cause analysis
6. Lessons learned
7. Response effectiveness
8. Opportunities for improvement
9. Identified gaps
10. Next steps and roadmap

## Communicating with the Board and Executives

- Be cautious about what is written down, it may be discoverable
- Anticipate Questions:
        - How much is this going to cost?
        - What this due to our negligence?
        - Did we handle this correctly once it was discovered?
        - What are we doing to prevent this from happening again?
- Focus on the future instead of the past
- Consider bringing in an outside consultant
- Careful about the amount of technical details you provide. Focus on mission, business, and risk

## Consider the CSF to communicate

![[CSF.png]]

## Plan of Action & Milestones (POA&M)

POA&Ms are used to identify, assess, prioritize and minotor corrective efforts for security weaknesses, deficiencies, and/or vulnerabilities found

![[poam.png]]

## Course Summary

- How to write a detailed incident response plan for an organization
- How to set an organization up for success prior to having an incident or breach to respond to 
- The people, processes, and technologies necessary to prevent, identify, detect, respond, and recovery from a cyber incident
- Collaboration and communication with internal stakeholders, vendors, partners, and external organizations during an incident
- The entire lifecycle of incident response from preparation to recovery
