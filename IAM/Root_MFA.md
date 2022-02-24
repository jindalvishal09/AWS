[<img alt="acosalens" width="200px" src="https://assets.zyrosite.com//YBgqZbnEvkulw8yL/Acosa_logo-A3Qn5vgEezFDLaJ7.png" />](https://acosalens.com)

# Securing Root User

## Quick Info

### _Why to secure a Root User?_

Root user is the only user in your AWS account which is unristricted and also can't be restricted as it is the super user of your account. In case your usrname/password get's compromised you will loose the complete control of your AWS account. So you need to 
1. Enable MFA
2. Delete all access keys for root user to disable programmatic  access from root user.

### _What is an Authentication Factor?_

An authentication factor is a special category of security credential that is used to verify the identity and authorization of a user attempting to gain access, send communications, or request data.

### _Five Authentication Factor Categories and How They Work_

1. Knowledge Factors :- Knowledge factors require the user to provide some data or information before they can access a secured system. a password or personal identification number (PIN).
2. Possession Factors :- Possession factors require the user to possess a specific piece of information or device before they can be granted access to the system.Like credit card, MFA Device
3. Inherence Factors :- Inherence factors authenticate access credentials based on factors that are unique to the user. These include fingerprints, thumbprints, and palm or handprints.
4. Location Factors :- Network administrators can implement services that use geolocation security checks to verify the location of a user before granting access to an application, network or system
5. Behavior Factors :- A behavior-based authentication factor is based on actions undertaken by the user to gain access to the system.Mobile phone lock-screens where the user is required to draw a specific pattern onto a grid of dots



## Detailed Remediation Steps

[Reference](https://www.sumologic.com/glossary/authentication-factor/)
