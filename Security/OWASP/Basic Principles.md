# 1. CIA Triad
 - **Confidentiality**: This principle focuses on restricting access to sensitive information to only authorized individuals or systems. It aims to prevent unauthorized disclosure and maintain the privacy of data.
 - **Integrity**: Integrity ensures that data is accurate, complete, and reliable, and that it has not been altered or destroyed improperly. It involves maintaining the trustworthiness of information.
 - **Availability**: This principle emphasizes the importance of ensuring that authorized users can access information and resources when they need them. It involves maintaining system uptime and preventing disruptions that could lead to data unavailability.
 # 2. AAA Model
 - **Authentication**: Who you are. There are someways to prove your identity: Something you know (password, secrect answer,...), something you have (key, smart card,...), something you are (fingure, eyes, face,...).
**MFA**: Multifactor authentication
 - **Authorization**: What you can do. 
 - **Accountability**: a set of policies to keep track of what users do while they are logged into a system
 # 3. NON Repudiation
Denying the truth or validity of something
# 4. Authorization and Permission
- Permissions: The rules of what actions a user or a software can perform on a specific system.
- Roles: A way of grouping together several related permissions into one package that can easily be assigned to a user.
- Main principles: least privileges, privilege escalation
# 5. Overview of Web application Security
- **Firewalls**: is a network security device that monitors and filters the incoming and outgoing network traffic based on a set of securiry rules. 
- **Limitations**: firewall does not protect the transported application protocols. HTTP and HTTPS ports can be use to encapsulate data for application platforms
- **DMZ (Demilitarized Zone)**: Physical or logical subnetwork that acts as a buffer between an internal local area network (LAN) from other unstrusted networks, such as the internet. The purpose of a DMZ is to add an additional layer of security to an oganization's local area network

# 6. Top 10 - 1: Broken object level authorization (B.O.L.A)
- Failing to validate if a user is allowed to access a particular object
- How to systems get caught by B.O.L.A: The use of increasemental IDs for Objects. Relying solvely on front-end restrictions
- How can we defend against B.O.L.A: Avoid predictable identifiers (UUIDs). Server-side authorization check. Minimizing data exposure. API Gateways. Continuous Monitoring. Educate and train development team.
# 7. Top 10 - 2: Broken Authentication
- The result of faulty implementations in the way a system verifies its users. Allowing unauthorized users to gain access to accounts that aren't theirs.
- Causes of broken authentication: weak session management (storing password in plain text). Exposed session IDs in the URL
- How to mitigate the risk of broken authentication: strong authentication Mechanisms (complex password, MFA). Implement session timeout. Hide session IDs. Server side check. Educate the team.
# 7. Top 10 - 3: Broken object property level authorization (B.P.L.A)
- Unauthorized to access to specific properties within objects.
- How do systems fall victim to B.P.L.A: over-reliance on front-end filtering. Lack of back-end verification. 
- How to mitigate: Fine-grained authorization. Server side data filtering. Training. Routine audits and Penetration testing.
# 8. Top 10 - 4: Unrestricted Resource Consumption
- An application doesn't have an appropriate controls to prevent users (or attackers) from consuming excessive resources. This can result in systems becomming slow, unresponsive, or event crashing entirely.
- How does this vulnerability present itself: lack of resource limits. Insufficient rate limiting. Abusing OTP feature
- Mitigation: rate-limiting. Resource consumption Caps. Connection Timeouts. Regular monitoring and alerts. Penetration testing and perfermance audits. Educate our team
# 9. Top 10 - 5: Broken function level authorization (B.F.L.A)
- Ensuring that users have the right to access and perform specific actions or functions in an application.
- Why does B.F.L.A occur: poorly implemented role check. Exposing admin endpoints. Insufficient session management. 
- Mitigation: strong role verification. Hiding sensitive endpoints. Proper session management. Regular secusiry audits. Educate our team.
# 10. Top 10 - 6: Unrestricted access to sensitive business flows
- Ensuring that certain core processes, specific to a business's operations, remain locked away from unauthorized users
- Why: Flawed workflow implementation. Overreliance on frontend security. Misconfigured API endpoints
- Mitigation: Robust workflow verification. Regular security review. Educate our team.
# 11. Top 10 - 7: Server side request forgery
- Attackers could potentially interact with internal system wich are normally shielded from the outside world, by taking adavatage of our server.
- Why: Misconfigured proxies and services. Over-trust in user input. Lack of Egress filtering. 
- Mitigation: Whitelist Urls. User input sanitization. Limit server permission. Monitoring. Educate our team.
# 12. Top 10 - 8: Security misconfiguration
- A system, application, or database is setup or deployed without proper security configurations.
- Why: Default configurations. Unnecessary features. Exposure of sensitive information. Outdated software. Hardening. 
- Mitigration: Limiting information Disclosure. Automated Scanners. Continuous Monitoring and patching. Regular configuration reviewss. 
# 13. Top 10 - 9: Improper inventory management. 
- The systematic tracking and oversight of all APIs throughtout their lifecyle.
- Why: rapid development cycles and resouce limitations. Inconsistent management and tool. Organizational changes and awareness.
- Mitigations: Clear definition of what constitutes an asset. Process for identifying and tracking assets. Produres for retiring assets. Regular audits of the asset inventory.
# 14. Top 10 - 10: Unsafe Consumption of APIs
- Ensuring that when our systems rely on external APIs those interations are secure and trustworthy.
- Why: Lack of validation. Over-reliance on external controls. Not considering API Dependencies
- Mitigration: Always validate data. Implement own set of security controls. Monitor API dependencies. Continuous education
# 15. Secure coding
Key strategies to enhance our code
- Clarifying Requirement
- Negotiating Deadlines
- Continuous learning 
The Vulnerability Cycle
- 
Why good developers Write bad code
- Human error
- Tight deadlines
- Complex requirements
- Inadequate testing
- Knowledge gap
