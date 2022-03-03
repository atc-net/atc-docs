# Infrastructure as Code (IaC)

`I`nfrastructure `a`s `C`ode (IaC) is the management of infrastructure (networks, virtual machines, load balancers, and connection topology) in a descriptive model, using the same versioning as DevOps team uses for source code. Like the principle that the same source code generates the same binary, an IaC model generates the same environment every time it is applied.

## Naming

As all resources in cloud environments are required to be globally unique, having naming rules and guidelines in-place becomes essential. The key to success with naming conventions is establishing and following them across your applications and organizations.

- ✔️ **Do** use abbreviations for long company and system names
- ✔️ **Do** have a naming standard in place
- 💭 **Consider** if the customer in question have some standard that needs to be enforced
- 💭 **Consider** the length of names for the different resources as different cloud vendors have different restrictions for this
- 💭 **Consider** the naming of services, which are utilizing the same base cloud service, e.g. in Azure its not possible to have the same resource name for Api, App, Azure Function - all using PaaS service - if hosted in the same resourcegroup, then they will be deployed into the same instance.

## Organize resources with tags

It is paramount to tag provisioned cloud resources as implementing a proper tagging strategy can help organizations gain much better control over and visibility of the resources that are hosted in their cloud vendors.

The tags can be anything that helps identify the category that a specific resource belongs to. For example, you can add environment-related tags to VMs to determine whether the machine belongs to the test, QA, or production environment.

### **Examples of tags**

|Tag|Meaning|
|---|---|
|CostCenter|Identifies the department responsible for paying for these resources|
|Owner|Who owns the resource|
|Env|Used to identify the environment type|
|System|Used to define the application or service|
|Repository/Source|Used to identify where these resources were provisioned from|

- ✔️ **Do** tag with CostCenter
- ✔️ **Do** tag with Environment
- ✔️ **Do** tag with System
- ✔️ **Do** tag with Repository/Source

## atc-snippets

When working with IaC - `Atc.Snippets` comes to the rescue for rapid scripting of deployment scripts or templates.

`Atc.Snippets` contains alot of script and template parts that can be combined or used directly. They only require inserting some project specific parameters and naming options.

## atc-azure-options

When working with IaC and `Atc.Snippets` teogether with some .NET code that uses `appsettings.json`, then the binding/mapping from json to code can be achieved by utilizing `Atc.Azure.Options`. This package contains binding-models and configuration method's to help with the setup in a Apps ConfigureServices method.
