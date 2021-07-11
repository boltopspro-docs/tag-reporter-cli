<!-- note marker start -->
**NOTE**: This repo contains only the documentation for the private BoltsOps Pro repo code.
Original file: https://github.com/boltopspro/tag-reporter-cli/blob/master/lib/tag_reporter/help/check.md
The docs are publish so they are available for interested customers.
For access to the source code, you must be a paying BoltOps Pro subscriber.
If are interested, you can contact us at contact@boltops.com or https://www.boltops.com

<!-- note marker end -->

## Example

    tag-reporter check

## Example with output

    $ tag-reporter check
    Required tags: Backup,Owner
    Resource types: AWS::EC2::Instance,AWS::EC2::Volume
    +--------------------+-----------------------+----------------+
    |    ResourceType    |      ResourceID       | Status        |
    +--------------------+-----------------------+----------------+
    | AWS::EC2::Instance | i-0eed378e45ef4e80c   | NONCOMPLIANT  |
    | AWS::EC2::Instance | i-0364992cef78f742c   | NONCOMPLIANT  |
    | AWS::EC2::Instance | i-065d6916cc44454d3   | COMPLIANT     |
    | AWS::EC2::Instance | i-07675908419abc7ed   | NONCOMPLIANT  |
    | AWS::EC2::Volume   | vol-03a027e0b000b3a77 | NONCOMPLIANT  |
    | AWS::EC2::Volume   | vol-09c019f828bdb20c4 | NONCOMPLIANT  |
    | AWS::EC2::Volume   | vol-0c3d2cdca30047660 | NONCOMPLIANT  |
    | AWS::EC2::Volume   | vol-0f835e4b3836acfe3 | NONCOMPLIANT  |
    | AWS::EC2::Volume   | vol-07e56fbe8f844cd3c | NONCOMPLIANT  |
    +--------------------+-----------------------+----------------+
    $