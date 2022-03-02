# Design practices

## Well-architected framework

Implementing Azure workloads with a DevOps mindset puts some requirements on the operational side of feature development. This includes aspects like cost control, security, performance, monitoring etc. The Microsoft well-architected framework consists of a set of guidelines for implementing Azure workloads. It touches importants areas sush as security, avalibility, resilience and scalability. It also has a range of reference architectures that can help as an inspiration when designing solutions.

[Microsoft Azure Well-Architected Framework](https://docs.microsoft.com/en-us/azure/architecture/framework)

## Agile planning

Agile Planning is the concept of handling user/customer requirements, changes and error related corrections and be able to prioritize and plan the delivery of these in continuous timeboxed iterations, while supporting team collaboration and continuous learning.

- ✔️ **Do** use an agile planning tool, that is integrated with the rest of the DevOps tools
    > *To achieve full traceability from requirement to deployed code in production, it is important to link requirements to code changes to builds and deployments in all environments. This automatically lifts the task of having change management on said environments and further documents why specific code changes were made and finally deployed to production*
- ✔️ **Do** comment directly on the requirements (work items) themselves
    > *To keep decision history close and traced*
- ✔️ **Do** breakdown task in sizes that can be handled in less than a day
- 💭 **Consider** breaking down requirements in three layers
    > *Use a structure like: Epics->Features->PBIs->Tasks.
Have business define their vision and roadmap via Epics and Features and make teams work on PBIs and Tasks.<br/>
When defining Epics, think months of work<br/>
When defining Features think weeks of work<br/>
When defining PBIs think days of work<br/>
When defining Tasks think hours of work*
- 💭 **Consider** having sprints (iterations) defined across teams
    > *So the same taxonomy and alignment can be used across teams. If more granular (shorter) iterations are needed for a team use sub division of the common iterations (like Sprint 1 and Sprint 1\Sprint 1.1 and Sprint 1\Sprint 1.2. This could be further exmplified; if two weeks sprints are used, use W2, W4, W6 etc as the common sprints and W2\W2.1 and W2\W2.2 for the team using one week sprints*
