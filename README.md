# byob

Script Downloads:

Gradle<br>
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.2/gradle-enterprise-gradle-build-validation-2.3.2.zip && unzip -q -o gradle-enterprise-gradle-build-validation-2.3.2.zip
<br>
Maven<br>
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.2/gradle-enterprise-maven-build-validation-2.3.2.zip && unzip -q -o gradle-enterprise-maven-build-validation-2.3.2.zip

<br>
How to invoke scripts:<br>
<br>
Gradle<br>
./03-validate-local-build-caching-different-locations.sh -r https://github.com/mockito/mockito -t build -e -s https://byob-devnexus-1.gradle-enterprise.cloud
<br>
Maven<br>
./02-validate-local-build-caching-different-locations.sh -r https://github.com/FasterXML/jackson-core -g install -e -s https://byob-devnexus-1.gradle-enterprise.cloud 
<br>
