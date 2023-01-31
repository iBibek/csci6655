# Adversary Engagement Ontology (AEO) #

>*"Adversary engagement is the combination of denial and
deception to increase the cost and decrease the value of your
adversary’s cyber operations. Adversary engagement goals can
be any combination of the following: to detect adversaries on
the network, to elicit intelligence to learn about adversaries,
or to affect adversaries by raising the cost and lowering the
value of their cyber operations - (MITRE Engage)"*

Adversary Engagement Ontology is the subontology of Unified Cyber Ontology that aims to define and standardize the information representation of the adversary engagement in cyber domain. 

- - - - 
## Objective ##
1.  To create a cyber adversary engagement subontology uder the UCO that  builds upon the concepts in MITRE’s open-source ENGAGE knowledge model but also seeks to expand into new areas of cyber adversary engagement between smart agents and the broad use of decoy and obfuscated data. 
2.  To establish a community of participants, with members from academia, government, non-profit, and for-profit organizations that participate in the engineering, adoption, and general support of the AE subontology

## Scope ##


## Approach ##
Adversary Engagement Ontology is a sub-ontology of the Unified Cyber Ontology (UCO. How the ontology is defined with an application space in CDO and why?

## Status ##
AEO is an initial draft and is not complete. We will be revising and making changes in the structure in upcoming days and many of the concept might be depreciated in future. If you wish to contribute, we highly encourage you to  join our community. Please visit aeo.sail-lab.org 

# Overview #

## Diagram ##


## Classes Tree ##
 ```
  ├── engage:Event
  ├── objective:Denial
  │    ├── objective:Trap
  ├── uco-action:Action
  │    ├── engage:Access
  │    ├── vengage:Alert
  │    ├── engage:Deploy
  │    ├── engage:Respond
  │        ├── engage:Obfuscate
  ├── uco-action:ActionLifecycle
  │    ├── attack:cyberKillChain
  ├── uco-action:ActionPattern
  │    ├── attack:AttackPattern
  │    ├── attack:DefensePattern
  ├── uco-core:UcoObject
  │    ├── engage:DataSource
  │    ├── engage:LureObject
  │    │     ├── engage:Breadcrumb
  │    │     ├── engage:Decoy
  │    │         ├── engage:Honeypot
  │    │     ├── engage:HoneyObject
  │    │         ├── engage:HoneyToken
  │    │         ├── engage:Honeypot
  │    ├── engage:Malware
  │    ├── engage:Narrative
  │    ├── engage:PlannedEvent
  │    ├── engage:PocketLitter
  │    ├── engage:Resource
  │    ├── engage:Sandbox
  │    ├── engage:Stage
  │    ├── engage:StageAttackSurface
  │    ├── engage:Storyline
  │    ├── objective:Objective
  │    |     ├── objective:Affect
  │    │     ├── objective:Collect
  │    │     ├── objective:CommandAndControl
  │    │     ├── objective:CredentialAccess
  │    │     ├── objective:Deny
  │    │     ├── objective:Detect
  │    │     ├── objective:DevelopResource
  │    │     ├── objective:Direct
  │    │     ├── objective:Discover
  │    │     ├── objective:Disrupt
  │    │     ├── objective:Elicit
  │    │     ├── objective:ElicitBehavior
  │    │     │       ├── objective:Lure
  │    │     ├── objective:Evade
  │    │     ├── objective:Execute
  │    │     ├── objective:Exfilitrate
  │    │     ├── objective:Expose
  │    │     ├── objective:Impact
  │    │     ├── objective:InitialAccess
  │    │     ├── objective:LateralMove
  │    │     ├── objective:Motivate
  │    │     ├── objective:Persist
  │    │     ├── objective:Prevent
  │    │     ├── objective:PrivilegeEscalate
  │    │     ├── objective:Reassure
  │    │     ├── objective:Reconnaissance
  │    │     ├── objective:TimeSink
  │    │     ├── objective:Track
  │    │     ├── objective:Trap
  ├── uco-identity:Identity
  │    ├── engage:Persona
  ├── uco-identity:Organization
  │    ├── role:Team
  ├── vocabulary:HoneypotInteractionTypeVocab
```

## Properties Tree ##
```
  ├── engage:alertContext
  ├── engage:eventContext
  ├── engage:hasCharacterization
  ├── engage:hasEvent
  ├── engage:hasStoryline
  ├── engage:honeypotInteractionType
  ├── objective:hasObjective
```
# Technical Detail # 

