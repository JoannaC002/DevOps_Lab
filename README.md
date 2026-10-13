# DevOps_Lab
mvn clean test and mvn package was used
branch name- feature

PS C:\Users\iot-a2\Downloads\Student-Starter\Student-Starter> git log --oneline
82dea25 (HEAD -> feature, origin/feature) Fixed Jenkinsfile-2
7b159df Fixed Jenkinsfile
90b1bf0 Adding Jenkinsfile outside
158d48e Adding Jenkinsfile outside
bd01925 Adding Jenkinsfile outside
3c8a9c0 Adding Jenkinsfile
cef2bff (main) Initial student assessment starter

Parent- child POM structure
child pom inherits the properties from the parent pom

 <parent>
        <groupId>com.university</groupId>
        <artifactId>course-registration-parent</artifactId>
        <version>1.0-SNAPSHOT</version>
        <relativePath>../pom.xml</relativePath>
    </parent>

given in child pom

maven is configured in jenkins.

jenkins follows an ordered flow
fetch verify test package deploy

if the build fails at any stage. it halts and does not proceed. therefore any test failure would stop the build before reaching package stage.

