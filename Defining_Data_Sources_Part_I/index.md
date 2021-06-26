**Defining ATT&CK Data Sources, Part I: Enhancing the Current State**

# overview
+ We almost talk about TTPs(Tactcs, Techniques, Procedures) but there are Data Sources too which are important
+ They provide valuable data for us for detections
+ In these 2 posts we'll talk about new methodology for defineing our `data sources` (part 1) and `data source objects` (part 2)

<div style="text-align:center">
	<img src="./images/data_source_objects.png" />
</div>

<br>

# Where to Find Data Sources Today
+ Data sources are featured as part of the **(sub)technique** object properties:
+ Current structure contains only names of data sources
+ To understand and effectively apply these data sources we should align them with our technologies, logs, sensors.

<div style="text-align:center">
	<img src="./images/LSASS_Memory_Sub-Technique.png" />
</div>

# Improving the Current Data Sources in ATT&CK
+ Data sources as defined in [mitre philosiphy](https://attack.mitre.org/docs/ATTACK_Design_and_Philosophy_March_2020.pdf):
	+ Information collected by sensors or Logging systems that may be used to collect information about adversaries actions and their results
+ ATT&CK Data Sources provide a relation beween adversary actions and our analysis. This makes it a vital aspect when developing detection rules
+ Here is a Number of Sub-Techniques per data source which most of them are about process and file monitoring

<div style="text-align:center">
	<img src="./images/DataSouces.png" />
</div>

## Develop Data Source Definitions
+ having definitions for data souces while contributing to data collection strategy developement enhances efficiency

<div style="text-align:center">
	<img src="./images/DataSources-map.png" />
</div>

## Standardize the Name Syntax
+ Data Sources can be interepretted differently. some are very specific like Windows Registery while others have wider scope

<div style="text-align:center">
	<img src="./images/Syntax.png" />
</div>

## Address Redundancy and Overlapping