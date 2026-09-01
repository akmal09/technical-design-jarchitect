# Technical Design Document Template for App

| **Project Code** |  |
| --- | --- |
| **Project Name** |  |
| **Project Jira Link** |  |
| **Requirement Document Link** |  |
| **IT Product Manager** |  |

# Background & Objectives

*\<insert the content here\>*

## **Background**

Explain Problem why the IC/RD is created and what is the problem that encountered by user/stakeholders.

## **Objectives**

*\<Explain what is problem that is need to be resolve with the objective with use case inside of it\>*

## **High Level Components**

### Client or Presentation Layer

*\<Describe client or presentation layer for solve the problem (usually frontend/mobile layer)\>*

### Application Layer

*\<Describe Application layer/backend for solve the problem.\>*

### Data Layer

*\<Describe data comoponents such as database, cache, storage, etc.\>*

### Infrastructure Layer

*\<Describe where the app/service is deployed and mechanism used to run inside platform (can be VM, containerized, physique server, etc)\>*

### Monitoring & Security Layer

*\<Describe which monitoring that used to operate the subsystem such as (grafana, tempo, open telemetry, etc)\>*


# Functional Architecture

| **Business Application Name** | *\<Please refer to the BIA Aplikasi list\>* |
| --- | --- |
| **Application System Name** | *\<insert the app system name here\>* |
| **Abbreviation** | *\<insert the app system code here, e.g. IALS\>* |

*\<Insert the diagram here, listing all of subsystem that involved in the project to solve the problem based on PRD/RD and give short explanation for the diagram too\>*



# Application Architecture

##  Subsystem Information

*\<Explain list of subsystem and what is used for every subsystem\>*

| **Name** | **New/Existing** | **Key Business Function** | **Detail Business Function** |
| --- | --- | --- | --- |
|  |  |  |  |
|  |  |  |  |

##  Current State Diagram

*\<Insert the diagram here, give explanation how the architeture system (high level) is exist\>*


##  Target State Diagram

*\<Insert the diagram here, give explanation how the architecture system is designed\>*


##  Sequence Diagram

*\<Insert every sequence diagram, the sequence diagram contain how every subsystem is interacted to run a business request\>*

##  Entity Relationship Diagram

*\<Insert an Entity Relationship Diagram (ERD) to define data architecute of the system in this project to solve problems from background and objectives. **This is optional section**\>*


##  Access Control Matrix

*\<Insert an Access Control Matrix/User Access Matrix to define what role and authorization inside the substem. **This is optional section**\>*

| **Role** | **Activity 1** | **Activity 2** | **Activity 3** | **Activity 4** | **Activity 5** |
| --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |
|  |  |  |  |  |  |

##  Proposed Options

Fill this table below if you have several options for the implementation of the technology 

*\<**This is optional section**\>*

| **1st Option** | **2nd Option** | **3rd Option** |
| --- | --- | --- |
| *\<Description* | *\<Description* | *\<Description* |
| Pros - xxx - xxx - xxx | Pros - xxx - xxx - xxx | Pros - xxx - xxx - xxx |
| Cons - xxx - xxx - xxx | Cons - xxx - xxx - xxx | Cons - xxx - xxx - xxx |



# Deployment Architecture

##  Diagram

*\<Insert the diagram here, this diagram is explained more detail from target state diagram section. This diagram contain where the subsystem/service is deployed from network segmentation (SF, DMZ, Public), infra/platform (VM, Kubernetes Cluster, Physique Server, etc)\>*

##  Resource Requirement

Please include all subsystem in the table below. If there’s no change in the subsystem, you do not required to fill the CPU, memory, and storage, but fill the Notes with “existing”. If you are using the existing server/node but require more resource, fill the CPU, memory, and storage with “before” and “after” and also fill the Notes with “need additional capacity”

If you have several option to implement the technology, please copy the table to create resource requirement per option

| **Subsystem Name** | **Instances** | **Bare metal / Virtual Machine /     Container** | **CPU** | **Memory** **(GB)** | **Block Storage (GB)** | **Object Storage** **(GB)** | **Notes** |
| --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |

##  Resiliency

|  |  |  |  |
| --- | --- | --- | --- |
| **Application Criticality** | * [ ] Critical  * [ ] High * [ ] Medium * [ ] Low | **DB Resiliency** | * [ ] Clustering  * [ ] Native replication * [ ] vSphere SRM * [ ] No Replication |
| **File Replication** | * [ ] using object storage native * [ ] using array replication * [ ] using software replication * [ ] no replication | **Backup DB Retention** | * [ ] 1 Week * [ ] 1 Month * [ ] 1 Year * [ ] 10 year |
|  |  | **Backup DB Frequency** | * [ ] Daily * [ ] Weekly * [ ] Monthly |

# Monitoring

| **Subsystem Name** | **Metrics** | **Logs** | **Trace** | **Dashboard** |
| --- | --- | --- | --- | --- |
|  |  |  |  | GRAFANAWECUBE |
|  |  |  |  | GRAFANAWECUBE |

# Additional Information

*\<insert additional information here\>*


# Enterprise Architecture Notes

##  EA Forum MoM Link

*\<insert Link here\>*


##  Technical Debt

| **Debt** | **Deadline** | **Work Item Link** |
| --- | --- | --- |
|  |  |  |
|  |  |  |
