# Publish To Bintray / JCenter
A very simple script to publish aar/jar to bintray/jcenter or common maven server

# How to use
1. edit **build.gradle** file in your project and add lines below:
```gradle
apply from: 'https://raw.githubusercontent.com/Rysle/PublishToBintray/master/publish.gradle'
```

2. create a new file named **publish.properties** in the same folder with **build.gradle**

3. edit **publish.properties** and add lines below
```gradle
# Group Id
POM_GROUP_ID=com.rysle.demo

# Artifact ID
POM_ARTIFACT_ID=library

# Artifact Version
POM_VERSION=0.0.1

# Artifact Packaging, i.e aar
POM_PACKAGING=aar

# Product Name
POM_NAME=Library Template

# Product Description
POM_DESCRIPTION=For Demo Only

# Product Url
POM_URL=https://github.com/Rysle/Library

# License, change to whatever you like
POM_LICENCE_NAME=The Apache Software License, Version 2.0
POM_LICENCE_URL=http://www.apache.org/licenses/LICENSE-2.0.txt
POM_LICENCE_DIST=repo

# Developer Info
POM_DEVELOPER_ID=Rysle
POM_DEVELOPER_NAME=Sky Lin
POM_DEVELOPER_EMAIL=N/A
POM_DEVELOPER_ORG=individual

# Project Url
POM_SCM_URL=https://github.com/Rysle/Library

# Project VCS Url
POM_SCM_CONNECTION=scm:git:git@github.com:Rysle/Library.git

# Project VCS Url
POM_SCM_DEV_CONNECTION=scm:git:git@github.com:Rysle/Library.git


# Maven Repo for Release
RELEASE_REPOSITORY_URL=

# Maven Repo for Snapshot
SNAPSHOT_REPOSITORY_URL=

# Maven Repo Username
REPOSITORY_USERNAME=

# Maven Repo Password
REPOSITORY_PASSWORD=


# Bintray Username
BINTRAY_USER_NAME=

# Bintray Maven Repo Name
BINTRAY_REPO_NAME=maven

# Bintray Package Name
BINTRAY_PKG_NAME=com.rysle.demo:library


# Where to publish to, can be bintray/local
SERVER=bintray

# Is this a snapshot build?
SNAPSHOT=false

# Should we upload artifacts after assembleRelease task?
AUTO_UPLOAD=false
```
