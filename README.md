# tAct1caL_1ncid3nt_Re5pons3
Incident Response is a task that any cyberwarrior will face somewhere in their expedition. Needing to know the basics will assist in eradicating the modern adversary. 

# Basic Attack Flow Diagram

![Breach-and-Attack](https://github.com/divandenyss/tAct1caL_1ncid3nt_Re5pons3/assets/156643542/6397f50e-368e-4087-a727-a49b4e8a9be9)
![Attack-Flow](https://github.com/divandenyss/tAct1caL_1ncid3nt_Re5pons3/assets/156643542/ad22240c-24fa-4d2a-8fbd-4f0164ac9c95)



# What is the "Source"? 
Threat Actors need access to your environment in some way, shape, or form. 
## Common Entry Points
- VPN, VPN, VPN
- Leaked Credentials
- Internet Facing Servers 
- Public Facing Management Ports (3389, 22, 5985, 21)
- Public Facing Login Interfaces

## Credentials are KING
The Incident Response Team needs to find and nuke the identity involved in the ongoing attacks. 
e.g. John Bridge (account being abused) accessed VPN and started with enumeration. John Bridge account should be nuked. 

## What does "nuke" account mean? 
- Disable On-Prem
- Remove Logon Hours
- Change password

