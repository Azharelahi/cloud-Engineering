# IaaS, PaaS, and SaaS

Cloud computing provides computing resources over a network instead of requiring an organization to own and maintain all of the underlying physical infrastructure. NIST defines three primary cloud service models: **Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS)**.

The easiest way to understand them is by looking at **who manages what**.

## 1. IaaS — Infrastructure as a Service

IaaS provides fundamental computing resources such as:

* Virtual machines
* Storage
* Networking
* Compute resources
* Other infrastructure components

The cloud provider manages the physical infrastructure, while the customer manages things such as the operating system, deployed applications, storage configuration, and selected networking components.

### Simple example

Instead of buying a physical server, I can create a virtual machine in Azure.

I am responsible for:

* Installing/configuring the operating system
* Installing my application
* Managing application dependencies
* Configuring the server
* Managing much of the security configuration

The cloud provider is responsible for the underlying physical servers, data center, and cloud infrastructure.

**Think:**

> "Give me the infrastructure. I will manage the software running on it."

---

## 2. PaaS — Platform as a Service

PaaS moves one level higher.

The cloud provider manages the underlying infrastructure, operating system, and platform components, while the developer focuses primarily on building and deploying the application.

For example, instead of creating a virtual machine and manually configuring a web server, I can deploy an application to a managed cloud application platform.

I primarily care about:

* My source code
* Application configuration
* Dependencies
* Application data
* Deployment

The provider handles much of the underlying infrastructure and platform management.

**Think:**

> "Give me a platform to run my application. I will focus on the application."

This is particularly useful for developers because it reduces the amount of infrastructure administration required.

---

## 3. SaaS — Software as a Service

SaaS is the highest level of abstraction.

The cloud provider delivers a complete software application that users access through a network, commonly through a web browser or application interface. The customer generally does not manage the underlying servers, operating systems, storage, or networking.

Examples include cloud-based applications such as:

* Email applications
* CRM systems
* Collaboration software
* Online document management systems

With SaaS, I generally don't care about the infrastructure running the application.

**Think:**

> "Just give me the finished software. I only need to use it."

---

## The Core Difference

The three models can be remembered as different levels of responsibility:

| Model    | Provider manages                    | Customer mainly manages               |
| -------- | ----------------------------------- | ------------------------------------- |
| **IaaS** | Physical infrastructure             | OS, applications, data, configuration |
| **PaaS** | Infrastructure + platform           | Application, data, configuration      |
| **SaaS** | Almost the entire application stack | Usage and limited configuration       |

The higher I move from IaaS → PaaS → SaaS, the more infrastructure management is abstracted away from me. NIST also describes these service models as hierarchical in terms of their management and access-control responsibilities.

## An Easy Analogy

Imagine I want to run a restaurant.

### IaaS

I rent an empty commercial kitchen.

I have the infrastructure, but I am responsible for setting up and managing most of what I need.

### PaaS

I rent a fully equipped kitchen.

The important infrastructure is already provided. I mainly focus on preparing and serving the food.

### SaaS

I order food from a restaurant.

I don't manage the kitchen, equipment, ingredients, staff, or infrastructure. I simply use the finished service.

---

## How This Relates to Azure

When learning Microsoft Azure, these three models help explain what Azure is actually providing.

For example:

**IaaS**

Azure Virtual Machines provide virtualized computing infrastructure that I can configure and manage.

**PaaS**

Managed application platforms allow me to deploy applications without having to manage the underlying servers and operating systems myself.

**SaaS**

A complete cloud application is provided to the end user, who primarily consumes the software rather than managing its infrastructure.

The important concept is not memorizing individual Azure services. It is understanding **the level of abstraction and responsibility** provided by each service model.

## My Mental Model

I can remember the three models like this:

**IaaS → Infrastructure**

> "I manage the machine."

**PaaS → Platform**

> "I manage my application."

**SaaS → Software**

> "I use the application."

This distinction is fundamental to understanding cloud computing and becomes increasingly important when designing, deploying, and operating cloud based systems.

### Key takeaway

IaaS gives me **infrastructure**.

PaaS gives me a **development and deployment platform**.

SaaS gives me **finished software**.

The fundamental tradeoff is between **control and management responsibility**: more control generally means more infrastructure responsibility, while higher-level services reduce infrastructure management.
