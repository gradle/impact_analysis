# Gradle Enterprise Impact Analysis
<br>
Welcome to the Gradle Enterprise Impact Analysis! This tool provides a streamlined method for understanding your project's build times, and build performance optimization potential. We can also use this tool to demo Gradle Enterprise to you with your own data, showing how Gradle Enterprise can help you improve build failure troubleshooting and build reliability. We'll work quickly to get you the information you need to 1) decide which projects to focus your build optimization efforts on and 2) build a business case for Gradle Enterprise using your real data.
<br>
Note: Be sure to make the correct selections for Gradle or Maven below

<br>
### If you have a full installation of Gradle Enterprise, do the following steps:

## Step 1: Get the build validation scripts

# Gradle
```bash
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.5/gradle-enterprise-gradle-build-validation-2.3.5.zip && unzip -q -o gradle-enterprise-gradle-build-validation-2.3.5.zip
```
# Maven
```bash 
curl -s -L -O https://github.com/gradle/gradle-enterprise-build-validation-scripts/releases/download/v2.3.5/gradle-enterprise-maven-build-validation-2.3.5.zip && unzip -q -o gradle-enterprise-maven-build-validation-2.3.5.zip
```
<br>

## Step 2: Invoke the scripts with your project and the server provided by your Gradle team

# Gradle Example
```bash
./03-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -t build -e -s https://<hostname>.gradle-enterprise.cloud
```

# Maven Example
```bash
./02-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -g install -e -s https://byob-devnexus-1.gradle-enterprise.cloud 
```

### If you are using the tool without a full installation of Gradle Enterprise, do the following steps:

## Step 1: Get the build validation scripts from your Gradle sales team

## Step 2: Invoke the scripts with your project and the server provided by your Gradle team

# Gradle Example
```bash
./03-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -t build -e -s https://<hostname>.gradle-enterprise.cloud
```

# Maven Example
```bash
./02-validate-local-build-caching-different-locations.sh -r <https://github.com/path/to/your/project OR file:///path/to/your/project> -g install -e -s https://byob-devnexus-1.gradle-enterprise.cloud 
```
<br>
NOTE: If you have any questions, please contact your Gradle team or use https://gradle.com/enterprise/contact/
<br>
