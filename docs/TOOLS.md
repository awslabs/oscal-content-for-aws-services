# Converting OSCAL JSON to OSCAL XML

[OSCAL CLI](https://github.com/metaschema-framework/oscal-cli) is an open source tool that can convert OSCAL content between the three OSCAL formats (XML, JSON, and YAML). 


# Acquisition

Download the latest version of the OSCAL CLI from [Maven](https://central.sonatype.com/artifact/dev.metaschema.oscal/oscal-cli-enhanced/versions) and follow these [installation instructions](https://github.com/metaschema-framework/oscal-cli?tab=readme-ov-file#installing). 


# Usage

To convert a file to a different OSCAL format using the Metaschema Framework OSCAL-CLI tool:

```
oscal-cli convert --to=<TARGET_FORMAT> <oscal_source_file> <oscal_target_file>
```
NOTES:
- The `<oscal_source_file>` can be any of the seven OSCAL models and any of the three OSCAL formats.
- The `<TARGET_FORMAT>` must be one of `XML`, `JSON` or `YAML`. (case sensitive)
- An optional `--overwrite` flag is used in scripts that perform the conversion. Otherwise, the tool will report an error if `<oscal_target_file>` already exists.


### Examples

To convert an AWS component definition from JSON to XML:
```
oscal-cli convert --to=XML --overwrite component-definitions/ec2.oscal.json ec2.oscal.xml
```

To convert the AWS Security Hub catalog from JSON to YAML:
```
oscal-cli convert --to=YAML --overwrite catalogs/aws_security-hub.oscal.json aws_security-hub.oscal.yaml
```
