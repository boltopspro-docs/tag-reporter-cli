<!-- note marker start -->
**NOTE**: This repo contains only the documentation for the private BoltsOps Pro repo code.
Original file: https://github.com/boltopspro/tag-reporter-cli/blob/master/README.md
The docs are publish so they are available for interested customers.
For access to the source code, you must be a paying BoltOps Pro subscriber.
If are interested, you can contact us at contact@boltops.com or https://www.boltops.com

<!-- note marker end -->

# TagReporter

[![Support](https://img.shields.io/badge/get-support-blue.svg)](https://boltops.com?utm_source=badge&utm_medium=badge&utm_campaign=session-manager)

[![BoltOps Badge](https://img.boltops.com/boltops/badges/boltops-badge.png)](https://www.boltops.com)

The tool checks for the presence of AWS resource tags on different types of resources. The list of tags is completely
configurable. The currently supported resource types are "AWS::EC2::Instance" and "AWS::EC2::Volume".

## Installation
```shell script
git clone git@github.com:boltopspro/tag-reporter-cli
cd tag-reporter-cli
bundle
```

## Usage
You need to set the tags to check for and resource types in tag_reporter.yaml file.

This the example configuration:
```yaml
required_tags:
    - Backup
    - Owner
resource_types:
    - AWS::EC2::Instance
    - AWS::EC2::Volume
```
The file can be placed in any of the following locations:
```shell script
./tag_reporter.yml
config/tag_reporter.yml
$HOME/.tag_reporter.yml
```

To run the check:

```shell script
exe/tag-reporter check 
```
You can also set an optional "status" flag ("COMPLIANT", "NONCOMPLIANT") to control if only compliant/noncompliant
resources should be displayed.
```shell script
exe/tag-reporter check --status=NONCOMPLIANT 
```