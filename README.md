# Microfrontends using vue and single-spa

## Overview
A micro frontend architecture with multiple Vue.js apps using single-spa. Note that you can replace Vue with your framework of choice.

## Goals
1. Having multiple decoupled applications running independently.
2. Each sub-application can be deployed independently and hosted on different servers.
3. Communication between sub-applications is possible.

## Implementation
![architecture](https://github.com/mpratap-dev/microfrontend-vue/blob/master/mfe.png?raw=true)

<p>In a nutshell: vendor dependencies get loaded from a CDN, app 1 and 2 bundles get loaded from S3/GCS and our container app composes/bundles it all together.</p>

## Steps to run the project

1. run `npm i` in each applications (i.e main, app-one, app-two)
2. run `npm run serve` in each project.
3. The app should be hosted at http://localhost:5000/
