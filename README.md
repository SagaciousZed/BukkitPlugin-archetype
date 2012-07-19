BukkitPlugin-archetype
===================

This is a Bukkit plugin maven archetype.
Bukkit is a Minecraft Server API.
Maven is a build system with dependency management.

Compilation and Installation
----------------------
This project uses maven to automate the build process.

* Install [Maven 3](http://maven.apache.org/download.html)
* Check out this repository
* In the projects root run `mvn install`

Usage
----------------------

Once installed, Maven can generate projects from this archetype. 

The standard way to generate projects is `mvn archetype:generate`, manually
searching for the archetype is less than ideal.

You can specify directly the archetype you want to use.

    mvn archetype:generate -DarchetypeGroupId=edu.neu.ccs.edpoon.bukkit -DarchetypeArtifactId=BukkitPlugin-archetype -DarchetypeVersion=0.0.2

It will still prompt you for additional important project information.

You can skip the prompt by supplying additional parameters appended to the call above

    -DgroupId=com.example.groupid -DartifactId=SampleBukkkitPlugin -Dpackage=com.example.groupid.samplebukkitplugin -Dversion=0.0.1-SNAPSHOT

Where `-DgroupId` specifies reverse domain name, if you don't have a domain 
name, use an email address. This is to uniquely name all your classes. 
DO NOT USE A *.me domain if you do not own it.

Where `-DartifactId` specifies the name of the project, this should be a
valid Java class name.

Where `-Dpackage` specifies the package for all the code, generally this is
the groupId.artifactId in all lower case.

Where `-Dversion` specifies the version, this should follow maven version
numbering convention. `[major].[minor].[revision]` the additional -SNAPSHOT
denotes that the revision is currently being worked on.

After maven generates the project it is ready to be imported into your IDE of choice.

Below is the complete call used to generate the BukkitSamplePlugin, which original source code
can be found at https://github.com/SagaciousZed/SampleBukkitPlugin

      mvn archetype:generate -DarchetypeGroupId=edu.neu.ccs.edpoon.bukkit -DarchetypeArtifactId=BukkitPlugin-archetype -DarchetypeVersion=0.0.2 -DgroupId=com.example.groupid -DartifactId=SampleBukkitPlugin -Dpackage=com.example.groupid.samplebukkitplugin -Dversion=0.0.1-SNAPSHOT