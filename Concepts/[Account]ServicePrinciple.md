# Service Principle
- Its a digital identity created for a software process rather than a person 
- Entry in a directory that allows a piece of code to prove its identity to a system


## Core Components 
The core components part of the service principle are: 
1. Unique identifier: ID that distinguishes it from other services 
2. Credentials: A way to prove the identity - usually a secret key, digital certificate or token 
3. Role/Permission: A list of what this identity is allowed to do

## Principle 
A "Principal" is any entity that can be authenticated.
- If a human authenticates, they are a User Principal
- If a service authenticates, it is a Service Principal

## How it works 
The process of using a Service Principal follows a standard handsshake:
1. The Identity Request: The software/application says to the security gatekeeper: "I am X, and here is my secret key."
2. Validation: The gatekeeper checks its database. If the secret matches X, it says, "Identity confirmed."
3. The Token: Instead of letting X keep the secret "open" all the time, the gatekeeper hands back a Session Token (like a temporary wristband).
4. Action: X shows the "wristband" to a database or API to perform its task.

## Difference between Service Account and Service Principle 
- While the "Service Account" is the record in the database, the Service Principal is the object that actually holds the permissions and performs the authentication.
- Service Account uses Username and password to login where as Service Principle uses Client Secret, Cert, or Federation.
- Passwords can be set up to last much longer


- Service Principle in Microsoft Entra ID is free 