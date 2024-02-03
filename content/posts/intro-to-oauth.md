---
title: "Intro to OAuth"
date: 2023-04-01T01:12:53+05:30
draft: true
---

## Why should I care?

## The Four Horsemen
- Resource Owner (User)
- Client/Application (Visitor)
- Authorization Server (Entrance Gate)
- Resource Server (Home)

## Outline
- Analogy
    - Performing OAuth2 for an application is like buying tickets to Disneyland
    - Resource Owner -> Disneyland's Owners
    - Client/Application -> Customers/Visitors
    - Authorization Server -> Ticket checking at the entrance
    - Resource Server - Disneyland
- Diagram
    - {{<figure src="https://drek4537l1klr.cloudfront.net/richer/Figures/01fig08_alt.jpg" caption="High-level overview of the OAuth Workflow" align="center">}}
- Example
- Plain English
- Technical Definition

### Steps
1. The application(you, the customer) requests authorization to access service resources from the user --> Buying tickets for Disneyland Online
2. If the user authorized the request, the application receives an *authorization grant* --> On successful booking, you receive tickets(auth grant)
3. The application requests an access token from the authorization server (API) by presenting authentication of its own identity(DL, Aadhar, PAN Card), and the authorization grant (Tickets)
4. If the application identity is authenticated and the authorization grant is valid, the authorization server (API) issues an ***access token*** (a band) to the application. Authorization is complete




