# byob

## Step 1: Get the Impact Analysis scripts

### Gradle
```bash
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.2/gradle-enterprise-gradle-build-validation-2.3.2.zip && unzip -q -o gradle-enterprise-gradle-build-validation-2.3.2.zip
```

### Maven
```bash 
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.2/gradle-enterprise-maven-build-validation-2.3.2.zip && unzip -q -o gradle-enterprise-maven-build-validation-2.3.2.zip
```

## Step 2: Invoke the scripts with your project and the server provided by your Gradle host

### Gradle
```bash
./03-validate-local-build-caching-different-locations.sh -r https://github.com/mockito/mockito -t build -e -s https://byob-devnexus-1.gradle-enterprise.cloud
```

### Maven
```bash
./02-validate-local-build-caching-different-locations.sh -r https://github.com/FasterXML/jackson-core -g install -e -s https://byob-devnexus-1.gradle-enterprise.cloud 
```
<br>
NOTE: 
<br>
<br>
The GE server used for these experiments is hosted by Gradle. It will be up until Apr 14, 2022, and then decommissioned. If you would want to continue with your own hosted instance, please reach out to us by using the following contact form:
<br><br>
https://gradle.com/enterprise/contact/
<br>
