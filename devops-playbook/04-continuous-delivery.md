# Continuous Delivery

`C`ontinuous `D`elivery (CD) is the process to build, test, configure and deploy from a build to a production environment. Multiple testing or staging environments create a Release Pipeline to automate the creation of infrastructure and deployment of a new. Successive environments support progressively longer-running activities of integration, load, and user acceptance testing. Continuous Integration starts the CD process and the pipeline is responsible for executing the deployment to each successive environments after successful completion of tests.

## Pipelines

One of the challenges of an automated build and test environment is you want your build to be fast, so that you can get fast feedback, but comprehensive tests take a long time to run. A deployment pipeline is a way to deal with this by breaking up your build into stages. Each stage provides increasing confidence, usually at the cost of extra time. Early stages can find most problems yielding faster feedback, while later stages provide slower and more throughout probing.

- ✔️ **Do** incremental provisioning of environments on every deployment
- ✔️ **Do** include database changes as part of your pipeline
    > *The database is a repository of the most valued and irreplaceable asset "our data" and preserving it accurately is imperative to continuous delivery.*
- ✔️ **Do** deploy the same way every time
    > *For a reliable process in all environments, then, the same set of steps must be repeated from start to finish. This ensures the same results in lower environments, with more frequent deployments (such as integration, QA, etc.), as in higher environments (pre-production and production), with fewer deployments.*
- 💭 **Consider** running smoke/integration/performance tests in parallel on separate environments
- 💭 **Consider** approval gates between environments to protect integrity and consistency
    > *UAT environments require a period where no new changes are allowed while manual tests are ongoing.*
- 💭 **Consider** provisioning a unique environment for performance tests and deleting after completion
    > *This is a more cost-effective approach and can facilitate performance tests in parallel for different releases.*
- 💭 **Consider** using continuous monitoring to automate release gates
    > *Gates allow automatic collection of health signals from external services, and then promote the release when all the signals are successful at the same time or stop the deployment on timeout.*
