# Infrastructure as Code (IaC)

`I`nfrastructure `a`s `C`ode (IaC) is the management of infrastructure (networks, virtual machines, load balancers, and connection topology) in a descriptive model, using the same versioning as DevOps team uses for source code. Like the principle that the same source code generates the same binary, an IaC model generates the same environment every time it is applied.

## Naming

As all resources in cloud environments are required to be globally unique, having naming rules and guidelines in-place becomes essential. The key to success with naming conventions is establishing and following them across your applications and organizations.

- ✔️ **Do** use abbreviations for long company and system names
- ✔️ **Do** have a naming standard in place

INPUT:

- restrictions on length of names for different resources and cloud vendors.
- restrictions within the customer you are currently working on
- Azure: restrictions on having e.g. same resource name for Api, App, Azure Function - all using PaaS service

## Organize resources with tags

It is paramount to tag provisioned cloud resources as implementing a proper tagging strategy can help organizations gain much better control over and visibility of the resources that are hosted in their cloud vendors.

The tags can be anything that helps identify the category that a specific resource belongs to. For example, you can add environment-related tags to VMs to determine whether the machine belongs to the test, QA, or production environment.

**Examples of tags**

|Tag|Meaning|
|-|-|
|CostCenter|Identifies the department responsible for paying for these resources|
|Owner|Who owns the resource|
|Env|Used to identify the environment type|
|System|Used to define the application or service|
|Repository/Source|Used to identify where these resources were provisioned from|

- ✔️ **Do** tag with CostCenter
- ✔️ **Do** tag with environment
- ✔️ **Do** tag with System
- ✔️ **Do** tag with Repository/Source

## atc-snippets

`TEXT-IS -MISSING`

## atc-azure-options

`TEXT-IS -MISSING`