# Development practices

`TEXT-IS -MISSING`


## Code quality

`TEXT-IS -MISSING`


### ATC coding rules

The ATC-Team have defined a setup for how to align on settings, rules, style etc. in a project / repository.

Benefits of this alignment setup that the ATC-Team endorses are special in:
- Enforce code styles. 
- Ensure less bugs.
- Ensure better performance.
- Ensure better design and maintainability of code.

The ATC coding rules setup is build and based on use of:
- [.editorconfig](https://editorconfig.org)
- [Directory.Build.props](https://docs.microsoft.com/en-us/visualstudio/msbuild/customize-your-build?view=vs-2022)

Read more on [ATC coding rules](https://github.com/atc-net/atc-coding-rules).
<br /><br />


### ATC coding rules updater

The [atc-coding-rules-updater](https://github.com/atc-net/atc-coding-rules-updater) is a cross platform command line application known as CLI tool.

The main purpose of this application is to create and maintain a project / repository with [ATC coding rules](https://github.com/atc-net/atc-coding-rules).
<br /><br />


## Source Control

`TEXT-IS -MISSING`


## Code review

`TEXT-IS -MISSING`


## Testing

`TEXT-IS -MISSING`


## Design for failure

`TEXT-IS -MISSING`


## Documentation

`TEXT-IS -MISSING`

## REST API design

`REST` is an acronym for `RE`presentational `S`tate `T`ransfer and an architectural style for `distributed hypermedia systems`.

`API` is the acronym for `A`pplication `P`rogramming `I`nterface, which is a software intermediary that allows two applications to talk to each other.

There exist lot of "Best practices for REST API design" on the internet
<br /><br />


### Design first approach (OpenAPI specification first)

There is to ways create an API:
- The `Code First` approach is a more traditional approach to building APIs, with the development of code happening after the business requirements are laid out, eventually generating the documentation from the code.
- The `Design First` approach advocates for designing the API’s contract first before writing any code. This is a relatively new approach, but is fast catching on, especially with the use of OpenAPI specification formats.

The philosophy behind the use of `Design First` as the `best approach` in the development and maintenance of an REST API is, to do it arraound a specification in a well know format as [OpenAPI specification](https://swagger.io/specification).

Benefits of this `Design First` approach that the ATC-Team endorses are special in:
- Empower technical and non-technical stakeholders to create and collaborate on API designs.
- `Server API` and `Client consumer` should agree around the specification before implementation - this saves time based on:
    - Single point of understanding of implementation strategy and maintenance.
    - Enforce the think, plan and execute over "try it out" strategy.
    - Enables better code documentation when good specifications are made.
    - Enables the options for parallel development of API and client(s).
    - Enables the options for code-generation to a specific language and/or framework.
    - Enables AGILE development with rapid development when using tools for code-generation.
    - Lot of OpenAPI specification tools already exist on the market.

Deficiencies that are often seen when using `Code First` approach:
- `Server API` and `Client consumer` is hard to keep in sync. and takes time in the implementation phase.
- It seems to be more fun in the startup phase for a developer, but happy-path is not always fun path in the long run.
- Developeres wants to code, but API's is not only about PoC's, and PoC's often have to be moved to production.

Recommended tools for working with OpenAPI specifications:
- [Stoplight.io](https://stoplight.io/)
- [OpenAPI extension for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=42Crunch.vscode-openapi)
<br /><br />


### ATC REST API Generator CLI Tool

The [atc-rest-api-generator](https://github.com/atc-net/atc-rest-api-generator) is a cross platform command line application known as CLI tool.

The main purpose of this application is to create and maintain a REST-API service based on an OpenAPI specification file. So the consept is the `Design First` approse.

And the `atc-rest-api-generator` should be categorized as a `Rapid Application Development Tool` for REST-API in .NET/C#.
