# Deployment Analysis: Virtual Machines vs Azure App Service

## Overview

In deploying the Article CMS application developed with the Flask framework in Microsoft Azure, two services were considered for deployment: **Virtual Machines** and **App Service**. These services have varying capabilities with regard to managing infrastructures, cost, and complexity of deployment and maintenance. The following section will briefly explain each of the services and the reason for the final choice of service for deployment.

---

# Virtual Machines

## Cost

Virtual Machines, as a service, requires a constant payment for compute resources as long as the machine is running. This includes CPU, memory, disk, and network resources.

## Scalability

In deploying an application using Virtual Machines, it is quite a challenge to scale up the application. This is due to the fact that a new machine instance has to be created and a load balancer set up.

## Availability

To ensure that the application is highly available, the application running in a Virtual Machine has to be set up for **Availability Sets** and **Availability Zones**. This is important so that the application is accessible by users and will not be taken offline by a machine failure.

## Workflow

To deploy an application in a Virtual Machine, a full operating system is required.

---

# Azure App Service

## Cost
The Azure App Service provides an environment that can host web applications. For a small-scale application like the Article CMS, options like Free and Basic are suitable. Azure provides an environment that can host web applications. This saves on costs since Azure takes care of all the costs involved in running a virtual machine.

## Scalability
The Azure App Service provides an environment that can scale up and down. This means that an application can increase in size vertically and horizontally. It can even automate scaling, thus making it easy to increase an application's size.

## Availability
The Azure App Service provides high availability. This means that an application hosted on Azure can always be available. This is due to the fact that Azure takes care of all server issues, thus making an application hosted on Azure always available.

## Workflow
The Azure App Service provides an easy deployment environment. This means that an application can easily be deployed on Azure. For example, an application can be deployed on Azure App Service. This means that developers can push an application, and Azure takes care of all the underlying infrastructure.

---

# Decision on Deployment
The Azure App Service has been chosen as the deployment environment for the Flask-based Article CMS.

The reason why Azure App Service has been chosen:
- It provides an easy deployment environment.
- It provides high availability.
- It provides scalability.
- It provides an easy deployment environment.
---
# When might we change our decision?
There are instances when we might change our decision. For example, if we need more control over our server, we might choose Azure Virtual Machine. This is because Azure Virtual Machine provides an environment that can install additional packages on an operating system.
