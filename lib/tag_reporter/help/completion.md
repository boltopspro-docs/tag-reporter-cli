<!-- note marker start -->
**NOTE**: This repo contains only the documentation for the private BoltsOps Pro repo code.
Original file: https://github.com/boltopspro/tag-reporter-cli/blob/master/lib/tag_reporter/help/completion.md
The docs are publish so they are available for interested customers.
For access to the source code, you must be a paying BoltOps Pro subscriber.
If are interested, you can contact us at contact@boltops.com or https://www.boltops.com

<!-- note marker end -->

## Examples

    tag-reporter completion

Prints words for TAB auto-completion.

    tag-reporter completion
    tag-reporter completion hello
    tag-reporter completion hello name

To enable, TAB auto-completion add the following to your profile:

    eval $(tag-reporter completion_script)

Auto-completion example usage:

    tag-reporter [TAB]
    tag-reporter hello [TAB]
    tag-reporter hello name [TAB]
    tag-reporter hello name --[TAB]
