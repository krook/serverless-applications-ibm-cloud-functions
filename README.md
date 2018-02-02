# Building serverless applications with IBM Cloud Functions

[IBM Cloud Functions](https://console.bluemix.net/openwhisk/) (powered by the open source [Apache OpenWhisk](http://openwhisk.incubator.apache.org/) project) is a public cloud platform for a new class of "serverless" applications composed of individual functions that typically run for a very short time, on-demand, and in response to unpredictable events or groups of events.

The key benefits of a serverless platform are:
* Automatic scale up and down to match demand with container lifecycle management handled by the system.
* A per execution cost model, matching the price paid directly to the resources used and value gained.
* Increased developer velocity thanks to a sharper focus on application features rather than operations.

What sets OpenWhisk apart from other serverless implementations is that it's an open source Functions-as-a-Service engine at its core and extremely flexible. That means it can be run in hybrid or edge scenarios, in addition to being consumed on the public cloud. It can be extended for additional runtimes and event source adapters. End users can see how data is stored and how it travels through the system.

This repository contains a curriculum, sample code, and reference architectures for building serverless applications with Apache OpenWhisk hosted as a service that powers IBM Cloud Functions. Its focus is on building applications with IBM Cloud Functions, rather than deploying them to Apache OpenWhisk on premises.

1. [Use cases](#1-use-cases)
2. [IBM Cloud Functions 101 - Getting started with serverless](#2-ibm-cloud-functions-101---getting-started-with-serverless)
3. [IBM Cloud Functions 201 - Other reference architectures](#3-ibm-cloud-functions-201---other-reference-architectures)
4. [IBM Cloud Functions 301 - Day to day development techniques](#4-ibm-cloud-functions-201---other-reference-architectures)
5. [IBM Cloud Functions 401 - Complete solution architectures](#5-ibm-cloud-functions-301---complete-solution-architectures)
6. [Resources](#6-resources)

## 1. Use cases
Serverless platforms are a great fit for existing cloud workloads, such as HTTP REST APIs, mobile backends, and UI-driven applications thanks to the attractive scale-on-demand model and efficient cost model.

Serverless platforms also bring bring the benefits of cloud computing (scale and cost) to a whole new range of applications that weren't a good fit for the HTTP-focused and daemon oriented Platform-as-a-Service, Containers-as-a-Service, and Infrastructure-as-a-Service models.

Applications that are a good fit for serverless architectures include those that process unpredictable data changes, analyze a firehose of IoT readings, implement asynchronous chatbots for millions of users, and run five-minutes-at-midnight batch jobs.

> **Note:** While there are indeed servers behind the scenes, the term serverless is popular because it highlights that the developer's point of view has shifted away from the operational aspects of what starts, runs, and scales his or her code. That, and because the application isn't always running in a daemon process awaiting user requests.


## 2. IBM Cloud Functions 101 - Getting started with serverless
Learn about the basic concepts behind serverless architectures, the OpenWhisk programming model, and deploy sample apps.

### Understanding serverless architectures
* [Five minute intro to open source serverless development with OpenWhisk](https://medium.com/openwhisk/five-minute-intro-to-open-source-serverless-development-with-openwhisk-328b0ebfa160)

### When to use a serverless approach instead of PaaS or containers
* [A look at using PaaS or container orchestration versus a serverless deployment model](https://www.slideshare.net/DanielKrook/containers-vs-serverless-navigating-application-deployment-options)
* [Additional context in the Cloud Native Computing Foundation whitepaper on serverless computing](https://docs.google.com/document/d/1UjW8bt5O8QBgQRILJVKZJej_IuNnxl20AJu9wA8wcdI/edit#heading=h.yiaul8is1ki)
* [When to use Serverless? When to use Kubernetes?](http://heidloff.net/article/when-to-use-serverless-kubernetes)

### Understanding how Apache OpenWhisk differs from IBM Cloud Functions
* Comparing IBM Cloud Functions to Apache OpenWhisk - TBD

### Getting started with some building blocks for common use cases
* [Building a basic function invocation on a fixed cron-style schedule](https://github.com/IBM/ibm-cloud-functions-scheduled-tasks).
* [Building a basic CRUD REST API call handler](https://github.com/IBM/ibm-cloud-functions-serverless-apis).
* [Building a basic message stream event processing system](https://github.com/IBM/ibm-cloud-functions-message-hub-trigger).
* [Building a basic database change event processing system](https://github.com/IBM/ibm-cloud-functions-cloudant-trigger).


## 3. IBM Cloud Functions 201 - Other reference architectures

### More complex versions of the basic use cases
* [Building a more complete REST API call handler](https://github.com/IBM/ibm-cloud-functions-serverless-apis).
* [Building a more complete a message stream event processing system](https://github.com/IBM/ibm-cloud-functions-data-processing-message-hubs).
* [Building a more complete a database change event processing system](https://github.com/IBM/ibm-cloud-functions-data-processing-cloudant).

### Other reference architectures
* Building a serverless web application - TBD
* Building a cognitive app to handle data at rest - TBD
* Building an interactive distributed processing application - TBD
* Bulding a map/reduce application - TBD
* Building a model-scoring application - TBD
* Building a Monte Carlo simulation - TBD
* Building a video processing application - TBD
* Building a mobile backend - TBD
* Building a serverless Express application - TBD
* Building an IoT message processing application - TBD
* Building a conversational bot - TBD


## 4. IBM Cloud Functions 301 - Day to day development techniques

### Debugging and monitoring applications
* TBD

### Zipped actions and custom Docker actions
* TBD

### Automation, declarative deployments with wskdeploy
* TBD

### Building complex workflows with Composer
* TBD

### Using the Shell
* TBD


## 5. IBM Cloud Functions 401 - Complete solution architectures

### Complete developer journeys that solve a particular problem with a complete solution
* [The full listing of IBM Code Patterns for serverless](https://developer.ibm.com/code/technologies/serverless/)

### OpenChecks
* [Serverless bank check deposit processing with object storage and optical character recognition using Apache OpenWhisk powered by IBM Cloud Functions.](https://github.com/IBM/ibm-cloud-functions-serverless-ocr-openchecks)

### BluePic
* [A sample photo sharing application for iOS that shows you how to connect your mobile application with Kitura, Bluemix services, and IBM Cloud Functions.](https://github.com/IBM/BluePic)

### OpenFridge
* [Improving customer service with IoT diagnostics and serverless, event-driven analytics.](https://github.com/IBM/ibm-cloud-functions-serverless-iot-openfridge)

### Skylink
* [A sample application that connects drones to the cloud with near realtime image analysis leveraging IBM Cloudant, IBM Cloud Functions and, IBM Watson services.](https://github.com/IBM-Cloud/skylink)

### Dark Vision
* [Discover dark data in videos with IBM Watson and IBM Cloud Functions](https://github.com/IBM-Cloud/openwhisk-darkvisionapp)


## 5. Resources

### Where to learn more and engage the Apache OpenWhisk community
* [Apache OpenWhisk official site](http://openwhisk.incubator.apache.org/)

### Where to get help and support from the IBM Cloud Functions service as a customer or partner
* [IBM Cloud Functions documentation](https://console.bluemix.net/docs/openwhisk/index.html#getting-started-with-openwhisk)
* [Engage an IBM developer advocate](https://developer.ibm.com/code/work-with-us)

### Finding, suggesting, and sharing your own journeys
* [IBM Code](http://developer.ibm.com/code/)
