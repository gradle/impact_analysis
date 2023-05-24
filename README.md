# Instructions for running the Impact Analysis
<br>
Note: Be sure to make the correct selections for Gradle or Maven below
<br>
<br>

## Step 1: Get the build validation scripts

### Gradle
```bash
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.5/gradle-enterprise-gradle-build-validation-2.3.5.zip && unzip -q -o gradle-enterprise-gradle-build-validation-2.3.5.zip
```

### Maven
```bash 
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.5/gradle-enterprise-maven-build-validation-2.3.5.zip && unzip -q -o gradle-enterprise-maven-build-validation-2.3.5.zip
```

## Note: If using the impact analysis in headless mode (without a full installation of Gradle Enterprise) see your Gradle sales team for these files

<br>

## Step 2: Invoke the scripts with your project and the server provided by your Gradle team

### Gradle Example
```bash
./03-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -t build -e -s https://<hostname>.gradle-enterprise.cloud
```

### Maven Example
```bash
./02-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -g install -e -s https://byob-devnexus-1.gradle-enterprise.cloud 
```
<br>
NOTE: If you have any questions, please contact your Gradle team or use https://gradle.com/enterprise/contact/
<br>
