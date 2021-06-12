# 1. Intro
+ Tactics (goals) and Techniques (How to reach goals) and Sub-techniques
+ History
	+ Started with FMX research by emulating labs and performing APT attacks and defenses
	+ ATT&CK for windows (2013)
	+ ATT&CK for macOS and Linux (2017)
	+ ATT&CK for mobile (2017)
	+ ATT&CK for cloud (2019)
	+ ATT&CK for ICS (Industrial Control Systems) (2020)


# 2. UseCases
+ Adversary Emulation
+ Red Teaming
+ Behavioral Analytics Development -> https://car.mitre.org/
+ Defensive Gap Assessment
+ SOC Maturity Assessment
+ Cyber Threat Intelligence Enrichment -> Don't categorise groups solely based on their use of TTPs

## 2.1 ATT&CK Coverage
+ Not possible to cover all techniques
+ No need to address all techniques (like checklists)
+ Example false positives
	+ ipconfig.exe in System Network Configuration Discovery in ATT&CK
	+ Domain or Local Account Usage
+ Important to review threat intelligence on what TTP's being used
+ Not possible to cover all Techniques and also Procedures


# 3. The ATT&CK Model
+ Set of Techniques and Sub-Techniques -> represent adversaries actions to achives Objectives (Tactics)
+ Actions occue at tactic level (why?!)

## 3.1 The ATT&CK Matrix
+ Include all Tactics and Techniques Example
+ Tactic : Persistence
	+ Technique : PreOS Boot
		+ Sub-Techniques :  (Bootkit, Component Firmware, and System Firmware)

## 3.2 Technology Domains
+ Domains are echosystems that adversaries are in
+ Three Technology Domains
	+ Enterprise
	+ Mobile
	+ ICS
+ Each Domain has several platforms (OS, Application Or ...)
+ PRE-ATT&CK defines behaviours before accessing and it's technology independant

|Technology Domain		|Platform(s) defined|
|:----------------------|:---------------|
|Enterprise				|Linux, macOS, Windows, AWS,Azure, GCP, SaaS, Office 365, Azure AD|ي
|Mobile					|Android, iOS														|

## 3.3 Tactics
+ Tactics represent `why` and goal of techniques and adversaries objectives
+ Treated as tags
+ each technique is tagged as one or more tactics

## 3.4 Techniques and Sub-Techniques
+ Techniques represent `how` to achive a tactical objective by performing actions and `what` they gain.
+ Sub-Techniques is details of a general Technique

### 3.4.1 Procedures
+ Implementations to do a specific technique like
	+ APT28 using PowerShell to inject into lsass.exe to dump credentials by scraping LSASS memory on a victim
+ It's how an adversary use several Techyniques and it's Sub-Techniques 
+ example for dumpiong credentials on a victim machine which is a Technique
	+ PowerShell, Process Injection and LSASS Memory
	
### 3.4.2 Technique and Sub-Technique Object Structure
+ Items are annotated by tag for filtering
+ Items are annotated by free text field for describing technique-specific information
+ Items marked with relationship indicate fields that are associated to object entity relationships with techniques or groups
+ Items with \* are `Required`


|Data Item				|Type				|Description|
|:----------------------|:------------------|:----------|
|Name*					|Field				|			|
|ID*					|Tag				|			|
|Sub-Techniques*		|Field				|			|
|Tactic*				|Tag				|			|
|Description*			|Field				|			|
|Platform*				|Tag				|			|
|System Requirements	|Field				|			|
|Permissions Required*	|Tag				|			|
|Effective Permissions*	|Tag				|			|
|Data Source*			|Tag				|			|
|Supports Remote		|Tag				|			|
|Defense Bypassed*		|Tag				|			|
|CAPEC ID				|Field				|			|
|Version*				|Field				|			|
|Impact Type*			|Tag				|			|
|Contributor			|Tag				|			|
|Procedure Examples		|Relationship/Field	|			|
|Detection*				|Field				|			|
|Mitigation*			|Relationship/Field	|			|

### 3.4.3 Sub-Technique Details
+ Adds scalability
+ reduce number of techniques and show different depths
+ makes abstraction level similar for all knowledge base
+ one-to-one relationship with Techniques (a bit odd)
+ Not all Techniques have Sub-Techniques
+ Sub-techniques are often but not always operating system or platform specific
+ Some information within a technique will be inherited by its child sub-techniques
+ Groups and software procedure examples are not inherited between techniques and sub-techniques

## 3.5 Groups
+ Represents known adversaries
+ Groups are defined as named intrusion sets, threat groups, actor groups, or campaigns that typically represent targeted, persistent threat activity
+ primarily focus on APT groups

### 3.5.1 Group Object Structure
+ Items are annotated by tag for filtering
+ Items are annotated by free text field for describing technique-specific information
+ Items marked with relationship indicate fields that are associated to object entity relationships with techniques or groups
+ Items with \* are `Required`

|Data Item							|Type				|Description|
|:----------------------------------|:------------------|:----------|
|Name*								|Field				|			|
|ID*								|Tag				|			|
|Associated Groups					|Tag				|			|
|Version*							|Field				|			|
|Contributor						|Tag				|			|
|Description*						|Field				|			|
|Associated Group Descriptions		|Field				|			|
|Techniques/Sub-Techniques Used*	|Relationship/Field	|			|
|Software							|Relationship/Field	|			|

## 3.6 Software
+ Softwares being used by adversaries
	+ Tools -> opensource, commercial, builtin and ...
	+ Malwares -> closedsource or opensource

### 3.6.1 Software Object Structure
+ Items are annotated by tag for filtering
+ Items are annotated by free text field for describing technique-specific information
+ Items marked with relationship indicate fields that are associated to object entity relationships with techniques or groups
+ Items with \* are `Required`
<br><br><br><br>

|Data Item							|Type				|Description|
|:----------------------------------|:------------------|:----------|
|Name*								|Field				|			|
|ID*								|Tag				|			|
|Associated Software				|Tag				|			|
|Version*							|Field				|			|
|Contributor						|Tag				|			|
|Type*								|Tag				|			|
|Platform*							|Tag				|			|
|Description*						|Field				|			|
|Associated Software Descriptions	|Field				|			|
|Techniques/Sub-Techniques Used*	|Relationship/Field	|			|
|Groups								|Relationship/Field	|			|

## 3.7 Mitigations
+ Solutions to prevent Techniques and Sub-Techniques
+ They are technology-based, not general solutions

### 3.7.1 Mitigation Object Structure
+ Items are annotated by tag for filtering
+ Items are annotated by free text field for describing technique-specific information
+ Items marked with relationship indicate fields that are associated to object entity relationships with techniques or groups
+ Items with \* are `Required`

|Data Item							|Type				|Description|
|:----------------------------------|:------------------|:----------|
|Name*								|Field				|			|
|ID*								|Tag				|			|
|Description*						|Field				|			|
|Version*							|Field				|			|
|Techniques Addressed by Mitigation*|Relationship/Field	|			|

## 3.8 ATT&CK Object Model Relationships
Shows Relationships between different models

<div style="text-align:center">
	<img src="file:///home/kourosh/mitre/attack/images/image1.png" />
</div>
<br>
<div style="text-align:center">
	<img src="file:///home/kourosh/mitre/attack/images/image2.png" />
</div>


## 3.9 Versioning
Standard versioning system for changes being applied in Techniques, Sub-Techniques and etc.
### 3.9.1 Objects
+ Indicates any item in the knowledge base that can have a relationship with another object
+ All objects are assigned a two part numerical version MAJOR.MINOR that starts at 1.0 for any new object

#### 3.9.1.1 Techniques and Sub-Techniques
+ MAJOR version changes include name and scope changes
+ Scope changes are how the Techniques could be interpreted and what they cover or does not cover and include to it's assigned tactics
+ MINOR version changes consist of relationships to Techniques and Groups

#### 3.9.1.2 Groups
+ Major version changes consist of changes or additions to associated groups as well as changes to the group’s description, which should happen infrequently.
+ Minor version changes consist of changes to references and relationships to techniques  and software.

#### 3.9.1.3 Software
+ Major version changes consist of changes or additions to associated software as well as changes to the software’s description
+ Minor version changes consist of changes to references and relationships to techniques and groups.

#### 3.9.1.4 Mitigations
+ Major version changes consist of changes to the scope of what the mitigation covers and changes to the name of the mitigation.
+ Minor version changes consist of changes to a mitigation’s description that does not impact its scope as well as changes to references and relationships to techniques.

#### 3.9.1.5 Deprecation
+ Objects may be deprecated when they have no more useful benefits like: combining technique ideas together or removing an unnecessary object.
+ Deprecated objects are not deleted from the knowledge base and are still maintained in the STIX repositories, but they no longer show up in the navigation bar and matrix within the main ATT&CK website.

### 3.9.2 Matrix
+ Each matrix has a last modified timestamp which is its version number
+ Relates to `Enterprise`, `Cloud`, `Mobile`, `PRE-ATT&CK`

### 3.9.3 Releases
Releases of all changes in github



# 4. The ATT&CK Methodology
+ Repsresents methodology used for maintaining of ATT&CK
+ Shows how categorise adversaries based on actions and relates them to sensors, system configs, countermeasures and ...

## 4.1 Conceptual
+ Maintains `adversary's prespective`
+ Follows real-world use of activity through `empirical`
+ The level of `abstraction` is appropriate

### 4.1.1 Adversary’s Perspective
+ Unlike many other security models that's based on defensive approaches, ATT&CK takes prespective of adversary's view
+ this makes it easy to understand what `could` happen in contrast to what `did` happen which the analytics have little sense and understanding of the alerts
+ It shows better view of Techniques and Tactics of an alert to understand the exact approach of attackers and theris goals

### 4.1.2 Empirical Use

ATT&CK is based on real world scenarios obtained from real adversary APT groups or offensive researches, so They're more likely to happen than theoretical techniques which are unlikely due to cost or difficulty.

#### 4.1.2.1 Sources of Information
The ATT&CK info are coming from different sources
+ Threat intelligence reports
+ Conference presentations
+ Webinars
+ Social media
+ Blogs
+ Open source code repositories
+ Malware samples


#### 4.1.2.2 Community Contributions
+ ATT&CK relies on community that analyze adversaries and attacks in the wild
+ One of the best sources are APT groups analyzers which makes new Techniques based on adversaries
+ Another great source is observations of defenders and analytics
+ Read teamers are another good good source because of developing new opensource softwares and ideas

### 4.1.3 Abstraction
+ Good level of abstraction is a nice feature of ATT&CK
+ Other security models abstraction level are good to understand the overall concept but not useful in understanding the detail Tatctics and Techniques being used by attackers and how they relates to softwares, groups, mitigations and etc. `(High level abstraction)`
+ Exploit and Malware databases are good too but don\t cover concepts like what area they're in and who are using them and how populer legitimate softwares can be used in malicious purpose `(Low level abstraction)`
+ A mid-level abtraction like ATT&CK helps to tie `high-level` concepts like **Control, Execute, Maintain** and `low-level` concepts like tools and exploits together and understand their area and usage to achive a specific goal and tactic.

<div style="text-align:center">
	<img src="file:///home/kourosh/mitre/attack/images/image3.png" />
</div>

**ATT&CK abstraction provides**
+ A common taxonomy of individual adversary actions and goals understood by both
offense and defense.
+ An appropriate level of categorization to relate adversary’s action and specific ways of
defending against it.

## 4.2 Tactics
+ Mainly remain static because tatctical goals are same
+ Exact similar tactics in Enterprise ATT&CK for different platforms(Windows, MacOS, Linux) and also for mobile devices with a few differenrces
+ Sometimes tactics need to be refined

### 4.2.1 Impact
+ Most tactics in ATT&CK were focused on data collection and exfiltriation
+ There was a lack of tactics which focus on destructive goals like ransomewares, DDoS, ...
+ So Impact tactic was added for this reason
+ Techniques and Sub-Techniques within **impact** Tactic include **Availability** or **Integrity** issues with a Tag labeled as `Availability` or `Integrity`



## 4.3 Techniques and Sub-Techniques
### 4.3.1 What Makes a Technique or Sub-Technique
There are several factor for Techniques and Sub-Techniques

#### 4.3.1.1 Naming
+ Names make techniques and Sub-Techniques unique
+ We've discussed example of a Tactic (Credential Access), Techniques (Credential Dumping) and Sub-Technique (use LSASS Memory)

#### 4.3.1.2 Types of Technique Abstraction
Techniques fall into 2 levels of abtraction
+ General Techniques applied to mutiple platforms in general way (like Exploiting Public Facing Application)
+ General Techniques applied to mutiple platforms in specific way (like Process injection which depends on the platform)

Sub-Techniques fall into 1 levels of abtraction
+ Specific way a techniques can be performed that may apply to 1 or more platforms (Rundll32 Sub-Technique as a specific way for Signed Binary Proxy Execution Technique)

+ Techniques that can be performed in mutiple ways to reach same or similar results are considered as one Technique and different Sub-Techniques based on platforms
+ Someimtes techniques and Sub-Techniques may have mutiple required steps

#### 4.3.1.3 Technical References
References related to Techniques like:
+ Background on the technique
+ Expected use in benign cases
+ General use examples
+ Variations of a technique
+ Relevant tools and open source code repositories
+ Detection examples and best practices
+ Mitigation categories and best practices

#### 4.3.1.4 Adversary Use
+ Techniques are based on threat groups and read tem researches (Data Source)
+ More Techniques for Windows than MacOS an Linux
+ There are several general categories of empirical use information that can be used:
	+ Reported
	+ Reported, non-public
	+ Underreported
	+ Unreported

#### 4.3.1.5 Technique Distinction
There are several factors for Techniques Distinction

+ Objective
	+ What the technique or sub-technique is accomplishing?
+ Action
	+ How a technique or sub-technique is performed?
+ Use
	+ Who is Using it?
+ Requirements
	+ The components that are needed to use a technique
+ Detection
	+ What needs to be instrumented to detect it
+ Mitigation
	+ What mitigation options available for the technique?


### 4.3.2 Creating New Techniques

### 4.3.3 Enhancing Existing Techniques
