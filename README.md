
# SKTWMS Platform v2

## Architecture Overview
![img](docs/images/SKTWMS Architecture.png)


## System Requirements
What we want is a new framework, not just a new website. The solution and design for that framework has to meet following requirements:

* Enterprise Scale Business requirements (Softketeers business)
    * Multiple services
    * Multiple user cases
    * Frequent business changes
    * Integrations
    * Support+++
      * Problem identify
      * Code fix
      * Time to delivery
* Modern development requirements
    * Modern technologies + Best practices: Main Stream
    * Productive: Fast/Effective/Work
    * Maintenance
## Technical Stack
* Back-End:
  * [ABP Framework](https://abp.io/): Open source
    web application framework
* Front-End
  * HTML 5/CSS3/JQuery
  * Bootstrap 4+
*  Infrastructure
    * .Net Core 6/latest
    * GitLab SC
    * GitLab CI/CD
*  Utility Services
    * Yarp gateway
    * Identity Server 4 security
    * Seq Logging
    * Redis Cache
    * ...

    
## Architecture Designs

### Software Architecture: Domain Driven Design (DDD) 
Domain-driven design (DDD) is an approach to software
development for **complex** needs by connecting the
implementation to an **evolving** model;

DDD is suitable for **complex domains** and **large-scale**
applications rather than simple CRUD applications. It **focuses
on the core domain logic** rather than the infrastructure details.
It helps to build a **flexible**, modular and **maintainable** code
base

![img.png](docs/images/abp/DDD Architecture.png)

* Business Logic places into two layers, the Domain layer and
the Application Layer
  * Domain Layer implements the core, use-case
  independent business logic of the domain/system.
  * Application Layer implements the use cases of the
  application based on the domain. A use case can be
  thought as a user interaction on the User Interface (UI).
* Presentation Layer contains the UI elements (pages,
  components) of the application.
* Infrastructure Layer supports other layer by
  implementing the abstractions and integrations to
  3rd-party library and systems

![img.png](docs/images/abp/Clean%20Architecture.png)

DDD mostly focuses on the Domain & Application Layers and
ignores the Presentation and Infrastructure.




> The **Key take-away** here: We find a software architecture (both technical and implementation) that help us to focus on our Core Business

### Application Architecture: Micro Services
Execution Flow of a DDD Based Application

![img.png](docs/images/abp/DDD%20execution%20flow.png)
## Technical Stack Details

### Abp Framework
![img](docs/images/abp/what-is-abp-framework.webp)
* Microservices Compatible
* Modular
* Background Jobs
* Cross-Cutting Concerns
* Best Practices
* Follow DDD/SOLID/Clean Architecture
* Community
* Documentation

[//]: # (![img_5.png]&#40;docs/images/abp/img_5.png&#41;)

[//]: # ()
[//]: # (![img_1.png]&#40;docs/images/abp/img_1.png&#41;)

[//]: # ()
[//]: # (![img_2.png]&#40;docs/images/abp/img_2.png&#41;)

[//]: # ()
[//]: # (![img_3.png]&#40;docs/images/abp/img_3.png&#41;)


### Implementation Structure

![img.png](docs/images/abp/Implemenation%20Strcture.png)

### Project Introduction

![img.png](docs/images/abp/Project%20Structure%20Introduction.png)

## Development Guide

For development, *see: [guidelines](docs/development_guide/development_guide.md)*


## References

* <a href="https://abp.io/" target="_blank">ABP framework</a>
* <a href="https://mega.nz/file/A6xwGbzS#DW5r9KoZkm5D5DhhPXdQuX31674HRKSm0w4OMKLbjPA" target="_blank">Implementing
  Domain Driven Design (DDD)</a>

