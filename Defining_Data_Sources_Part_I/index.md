**Defining ATT&CK Data Sources, Part I: Enhancing the Current State**

# overview
+ We almost talk about TTPs(Tactcs, Techniques, Procedures) but there are Data Sources too which are important
+ They provide valuable data for us for detections
+ In these 2 posts we'll talk about new methodology for defineing our `data sources` (part 1) and `data source objects` (part 2)

![[./images/data_source_objects.png]]

<br>

# Where to Find Data Sources Today
+ Data sources are featured as part of the **(sub)technique** object properties:
+ Current structure contains only names of data sources
+ To understand and effectively apply these data sources we should align them with our technologies, logs, sensors.

![[./images/LSASS_Memory_Sub-Technique.png]]
