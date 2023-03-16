# Maven Archetype for Micro Focus Data Protector UIC Plugin

This project is a [Maven Archetype](https://maven.apache.org/archetype/) project that can be used to create the
skeleton project structure and stub files for the development of *UIC plugin* for *Micro Focus Data Protector*. 

## Installing the archetype
* Clone or download the project.
* Make sure that you have JDK 17 and recent version of Maven installed.
* Run `mvn clean install` in the root of the project. This will build and install the archetype on the local machine.

## Using the archetype
* cd to a directory where you want to create a new plugin project
* Run `mvn archetype:generate -DarchetypeGroupId=com.microfocus.dp -DarchetypeArtifactId=uic-plugin-archetype -DarchetypeVersion=1.0.0` and enter appropriate input values for the properties when prompted. Here's an example:

![Screenshot](images/generate_project.png?raw=true)

&nbsp;&nbsp;&nbsp;&nbsp;IMPORTANT: For the property *pluginNameLowerCase*, do not enter value. You must accept the default value presented.

## Using the generated project
Refer to the README.md in the root of the generated project for instructions on how to use the skeleton project to develop, build, deploy, and run a plugin.

## Example plugin
This project also contains an example plugin named **SampleFS** (in *examples/samplefs-plugin* directory). The *SampleFS* plugin is developed using the skeleton project created from the archetype and adds rudimentary backup and restore functionality for a directory on the file system. See *examples/samplefs-plugin/README.md* for more details.

## What's new
- 1.0.0
    - Initial release
    
## License
[MIT license](LICENSE).

## Disclaimer