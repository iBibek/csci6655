# Adversary Engagement Ontology (AEO) #

>*"Adversary engagement is the combination of denial and
deception to increase the cost and decrease the value of your
adversary’s cyber operations. Adversary engagement goals can
be any combination of the following: to detect adversaries on
the network, to elicit intelligence to learn about adversaries,
or to affect adversaries by raising the cost and lowering the
value of their cyber operations - (MITRE Engage)"*

Adversary Engagement Ontology is the subontology of Unified Cyber Ontology that aims to define and standardize the information representation of the adversary engagement in cyber domain. AEO also aims to standardize and simply documentation and transmission of deployment configuration of cyber adversary engagement tools and techniques.  


## Objective ##

1.  To create a cyber adversary engagement subontology uder the UCO that  builds upon the concepts in MITRE’s open-source ENGAGE knowledge model but also seeks to expand into new areas of cyber adversary engagement between smart agents and the broad use of decoy and obfuscated data. 
2.  To establish a community of participants, with members from academia, government, non-profit, and for-profit organizations that participate in the engineering, adoption, and general support of the AE subontology

## Scope ##
The concepts and objects in the AEO are related to adversary engagement, however many of the contents are shared between CTI ontology and the concepts that may be added in the UCO in future. 
In this case, we may depreciate the existing classes and can add more, which will break out examples. 


## Approach ##

AEO is detined as an application domain ontolog within the Linux Foundation Cyber Domain OntoloR project and conformant with the Unitied cyber Ontology ecosystem.

## Status ##
The current version of AEO is 0.0.4. We will be working



- - - - 

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


## Technical Details ## 


### Dependencies 
```
- python 3.7 
- ontospy 2.1.1
- jinja2 3.1.2
- UCO 1.0.0

```

### Installation 

1. Run ``` pip install -r requirements.txt ``` . 
Warning:  Be aware that Jupyter Notebook may break in Anaconda

2. Run ``` pip install --upgrade nbconvert``` 
3. Run ```pip install mistune==0.8.4```


## How to regenerate Adversary Engagement Ontology ? 
1. Run `python code/gen_ontology.py`
2. Run `python code/owl_generator.py ontology`
3. Run `ontospy gendocs ae_ontology.ttl`

### How to generate HTML docs ? ###
1. Generate single owl file from folder `code` and then run `python owl_generator.py ../ontology`
2. Generate docs via gendocs. `ontospy gendocs code/ae_ontology.owl` Warning: Do not generate in working directory this will break `.git/HEAD`
