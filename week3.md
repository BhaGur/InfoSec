# Week 3 assignment
This file contains the tasks for the week 3 ATT&CK of security information course. Here, I have summarized the ATT&CK Framework and described few of the terminology.
## Chapter 4: Mapping the Adversary
### ATT&CK Framework
* It is important to have a good threat intelligence in order to have an effective threat hunting.
* ATT&CK framework is used to label and study the activities of the threat actors.
* Adversary behaviors are defined by both offensive and defensive researchers and communicated with people who do not have specialization in the field.
*	The framework allows to build your own tactics, techniques, and procedures (TTPs) and share them with others.
*	ATT&CK enterprise have categorized 14 tactics, each having a tactical goal, using different set of techniques.
*	Reconnaissance, Resource Development, Persistence, Defense Evasion are few of the tactics used.
*	Each tactic describes specific threat actor behaviors.
*	The framework divides techniques and sub-techniques into different categories.
*	There are 183 techniques and about 372 sub-techniques recorded.
*	Procedure is a specific way that the threat actor uses to implement a technique or sub-technique. A single procedure can expand into multiple techniques and sub-techniques.

### ATT&CK Matrix
*	It is important to understand the structure and navigation of the matrix to identify the threat behaviors.
*	The Matrix has a tactics as its column heading and the list contains the techniques under each tactic.
*	Some of the techniques expand to sub-techniques.
*	All the information about the technique, such as sub-techniques, platforms it operates on and data sources can be read.
*	Recommended detections and a list of mitigations to prevent the technique can also be found.

<img src="https://github.com/BhaGur/InfoSec/blob/main/attack1.png" > 


### ATT&CK Navigator
*	The tool is used to visualize threat actor’s modus operandi, the behavior of the specific tool ir to generate security exercises.
*	The tool allows us to create layers and study about them and give scores. 

## Mitre Att&ck
### Tactic
Tactic is an action performed by the threat actors to achieve a specific goal. It represents the “why” of an ATT&CK. Reconnaissance is one of the examples of a tactic used by the adversary. The adversary gathers information which can be used to plan an action in the future. There are many techniques that an adversary uses in this tactic. They are passively or actively gathering information about the details of the victim. Some of the techniques used are active scanning, gather victim identity information, gather victim organization information.
### Technique and Sub-technique
Technique represents the method used by the adversary to achieve a tactical goal. It represents the “how” of an ATT&CK. Technique can branch out to have multiple sub-techniques. In Reconnaissance, adversary uses Active Scanning technique to gather information that can be used during targeting. There are 3 sub-techniques of Active Scanning. One of the sub-technique is Scanning IP Blocks where adversary scans victim’s IP blocks to gather information. Scans may range from simple pings to more nuanced scans that reveals as host software/versions.
### Procedure
Procedure is a specific way adversary uses to implement the technique of sub-technique. Adversaries scan IP blocks to gather victim network information such as IP addresses that are actively in use.


