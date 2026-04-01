# Experimental AWS OSCAL Content

Amazon Web Services (AWS) is offering _experimental_ Open Security Controls Assessment Language (OSCAL) content for public review and feedback. This OSCAL package is experimental and may contain errors or inconsistencies with other published information. Future versions of this OSCAL content, if any, may not be backwards compatible. 

## Available Content

This repository contains OSCAL content in JSON format conforming to OSCAL version 1.2.1. The content is organized into the following directories:

### Catalogs

The [`catalogs/`](catalogs/) directory contains OSCAL catalog files. Currently this includes the AWS Security Hub Controls catalog with 77 groups and 452 controls. See the [Catalogs README](catalogs/README.md) for details.

### Component Definitions

The [`component-definitions/`](component-definitions/) directory contains 230 OSCAL component definition files describing AWS regions and services. Each AWS service is modeled as a _component_ within a file. Service components with Security Hub controls include references to the [catalog](catalogs/aws_security-hub.oscal.json) and associated Config rules. 

See the [Component Definitions README](component-definitions/README.md) for a full inventory, or the [AWS Component Definitions](docs/COMPONENTS.md) document for details on the OSCAL representation.

### Tools

See the [Tools](docs/TOOLS.md) document for information on converting OSCAL content between formats.

## Additional Resources

You may also want to try the [OSCAL MCP Server](https://github.com/awslabs/mcp-server-for-oscal/), which can help you understand the content in this project, how to use it, and OSCAL in general. 

## We want to hear from you!
Our goals for this experiment are to understand customer interest and use-cases for machine-readable compliance artifacts. To that end, AWS needs your feedback about the quality and usefulness of this content.
If you have questions, suggestions or concerns, please [open an issue](https://github.com/awslabs/oscal-content-for-aws-services/issues/new).


## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This project is licensed under the [Apache-2.0 License](LICENSE).
