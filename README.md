# tAct1caL_1ncid3nt_Re5pons3
Incident Response is a task that any cyberwarrior will face somewhere in their expedition. Needing to know the basics will assist in eradicating the modern adversary. 

# The simplified concept behind Incident Response
To simplify it, hackers/adversaries, and threat actors need access to your environment and they need credentials to perform their malicious tasks internally. 
Below is a guide that will aid in investigation and eradication. 

# Basic Attack Flow Diagram

![Breach-and-Attack](https://github.com/divandenyss/tAct1caL_1ncid3nt_Re5pons3/assets/156643542/6397f50e-368e-4087-a727-a49b4e8a9be9)
![Attack-Flow](https://github.com/divandenyss/tAct1caL_1ncid3nt_Re5pons3/assets/156643542/ad22240c-24fa-4d2a-8fbd-4f0164ac9c95)


# FInd the "Source"? 
Threat Actors need access to your environment in some way, shape, or form. 
## Common Entry Points
- VPN, VPN, VPN
- Leaked Credentials
- Internet Facing Servers 
- Public Facing Management Ports (3389, 22, 5985, 21, 445, 189, 389)
- Public Facing Login Interfaces

# Break the "source", "service" and "identity" 
E.g. Lets say you are traveling to a foreign country by road. For you to get there, you need a passport, a road, and a car. 
The road, in this case, is the "source", your passport is the "identity", and the car is your "service".
- Removing the "road/source" will cut comms and connection.
- Nuking the "passport/identity will ensure no further lateral movement or enumeration
- Cutting the "car/service" will ensure no further connection, as same with "source"

![Simplified View](https://github.com/divandenyss/tAct1caL_1ncid3nt_Re5pons3/assets/156643542/86391977-1dfe-49b5-acf9-d74456ffdf60)


## Credentials are KING
The Incident Response Team needs to find and nuke the identity involved in the ongoing attacks. 
e.g. John Bridge (account being abused) accessed VPN and started with enumeration. John Bridge's account should be nuked. 

## What does "nuke" account mean? 
### On-Prem
- Disable Account
- Remove Logon Hours
- Change password

### In the Cloud
- Revoke Session, this will kick the unwanted actor out of all logged-in applications.
- Change password
- Create a tactical group, that has conditions. e.g. Create a group, anyone in that group should be denied access to any cloud resource as part of a Conditional Access Policy (If using Entra ID) 

