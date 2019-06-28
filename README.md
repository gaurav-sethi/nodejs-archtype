Mule Ascendon TIger API Maven Archetype
======================================

Summary
-------
The project is a Maven archetype for CSGI - Ascendon Tiger API application.

Generated project characteristics
-------------------------
* RAML file
* Mule Flows GET,POST, DELETE and PATCH
* Munit

Prerequisites
-------------

- JDK 8
- Maven 3

Create a project
----------------

```bash
    mvn archetype:generate \
        -DarchetypeGroupId=org.ascendon.common \
        -DarchetypeArtifactId=ascendon-mule-archetype \
        -DarchetypeVersion=1.0.0-SNAPSHOT \
        -DgroupId=org.acendon \
        -DartifactId=asendon-s-demo \
        -Dversion=1.0.0-SNAPSHOT
        -DprojectName=demo
        
        Note ignore entering values for projectNameTitle and projectNameLowerCase.
 
```

Note: The above command will bootstrap a project using the archetype published here: Gerri Path

Run the project
----------------

Navigate to newly created project directory (`artifactId`) and then run:
You can build the project and run the tests by running ```mvn clean package```

Import the project in anypoint studio and run by adding envriorment variable mule.env=Local in Run Configurations.




Test in the browser
-------------------

	http://localhost:8081/demo/find/123


Install archetype locally
-------------------------

To install the archetype in your local repository execute the following commands:

```bash
    git clone http://username@http://devops.gitpath/gerrit/ascendon-archetype.git
    cd ascendon-archetype/ascendon-mule-archetype
    mvn clean install
```

Create a project from a local repository
----------------------------------------

Create a new empty directory for your project and navigate into it and then run:

```bash
   mvn archetype:generate \
        -DarchetypeGroupId=org.ascendon \
        -DarchetypeArtifactId=ascendon-mule-archetype \
        -DarchetypeVersion=1.0.0-SNAPSHOT \
        -DgroupId=org.ascendon \
        -DartifactId=ascendon-s-demo \
        -Dversion=1.0.0-SNAPSHOT
        -DprojectName=demo
        
        NOte ignore entering values for projectNameTitle and projectNameLowerCase.
```

Note: The above command will bootstrap a project using the archetype published in your local repository. 

mvn org.apache.maven.plugins:maven-archetype-plugin:2.0-alpha-4:generate -DarchetypeGroupId=org.ascendon.common -DarchetypeArtifactId=ascendon-mule-archetype -DarchetypeVersion=1.0.0-SNAPSHOT -DgroupId=org.ascendon -DartifactId=ascendon-s-demo -Dversion=1.0.0-SNAPSHOT -DprojectName=demo
