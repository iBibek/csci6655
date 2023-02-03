# Adversary Engagement Ontology (AEO) #

Adversary Engagement Ontology (AEO) is a sub-ontology of the Unified Cyber Ontology that focuses on defining and standardizing the information representation of adversary engagement in the cyber domain. Adversary engagement is the strategic use of denial and deception tactics aimed at increasing the cost and decreasing the value of an adversary's cyber operations ([MITRE ENGAGE](https://engage.mitre.org/)). The goals of adversary engagement can include detecting adversaries on a network, eliciting intelligence about them, or affecting them by raising the cost and lowering the value of their cyber operations.

AEO aims to standardize and simplify the documentation and transmission of the deployment configuration of cyber adversary engagement tools and techniques. This helps to ensure a consistent and efficient approach to adversary engagement across different organizations and domains. The standardization provided by AEO enables better collaboration and sharing of information among stakeholders, leading to more effective adversary engagement.


## Objective ##

1. The Adversary Engagement Ontology (AEO) aims to establish a sub-ontology within the Unified Cyber Ontology (UCO) that incorporates and expands upon the foundational concepts found in MITRE's open-source ENGAGE and ATTACK knowledge models. The ultimate goal is to advance the field of cyber adversary engagement by exploring new avenues, including the interactions between smart agents and the implementation of decoy and obfuscated data.
2. The Adversary Engagement Ontology (AEO) endeavors to bring together a diverse and inclusive community of stakeholders, comprising members from academia, government, non-profit, and for-profit organizations, to actively participate in the development, implementation, and sustained support of the Adversary Engagement (AE) sub-ontology.


## Scope ##
The Adversary Engagement Ontology (AEO) focuses on the subject matter pertaining to engaging with adversaries. Drawing upon concepts from the Unified Cyber Ontology (UCO), MIRE ATTACK, and MITRE ENGAGE, the AEO selectively incorporates relevant ideas and categories. Additionally, there exist several concepts that overlap with the Cyber Threat Intelligence (CTI) ontology and other domains within cybersecurity. The AEO strives to encompass only those concepts that are directly related to adversary engagement and does not aim to be all-inclusive.


## Approach ##

AEO is detined as an application domain ontolog within the Linux Foundation Cyber Domain OntoloR project and conformant with the Unitied cyber Ontology ecosystem. 

## Status ##
This is the AECO v 1.0.0 . We will be making changes in future by adding new concepts and depreciating the current concepts based on the community suggestions. If you would like to contribute we highly encourage you to join our community. You can get more details [here](https://aeontology.sail-lab.org/)



- - - - 

# Overview #

There are 65 Classes and 7 properties in the AEO. The Classes Tree and Properties Tree are listed below. 

![alt text](https://github.com/UNHSAILLab/ae_ontology/blob/main/ae_diagram.PNG?raw=true)

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

