# omar-ossimtools

[![Build Status](https://jenkins.radiantbluecloud.com/buildStatus/icon?job=omar-ossimtools-dev)]()

### Required environment variable
- OMAR_COMMON_PROPERTIES

### Optional environment variables
Only required for Jenkins pipelines or if you are running Artifactory and/or Openshift locally

- OPENSHIFT_USERNAME
- OPENSHIFT_PASSWORD
- ARTIFACTORY_USER
- ARTIFACTORY_PASSWORD

## How to Install omar-ossimtools-app locally

1. Install omar-oms-plugin [click this link for instructions](https://github.com/ossimlabs/omar-oms)

2. Git clone the following repos or git pull the latest versions if you already have them.
```
  git clone https://github.com/ossimlabs/omar-geoscript-plugin.git
  git clone https://github.com/ossimlabs/omar-ossimtools.git
```

3. Install omar-geoscript-plugin
```
 cd omar-geoscript/plugin/omar-geoscript-plugin
 ./gradlew clean install
```

4. Build/Install omar-ossimtools-app
#### Build:
```
 cd omar-ossimtools/apps/omar-ossimtools-app
 ./gradlew clean build
 ```
#### Install:
```
 cd omar-ossimtools/apps/omar-ossimtools-app
 ./gradlew clean install
```
