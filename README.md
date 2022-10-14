# Redbill Scanner - magic-stack


How this works?

You click a button, and RedBill gets an email with the amount that can be easily saved across your entire AWS organization.

The fixers are purely financial in nature, meaning the fixing part is both easy and:
* No risk of downtime to your resources, applications and systems
* No unexpected outages due to configuration changes
* No complexity of changing hundreds or thousands of resources

Transparency:

Redbill Magic Stack does not require any access to your account in the initial scan. The Scan simply outputs potential, so
we are sure there are easy savings to be made, before we even contact you.

You can delete the stack at any time.

> **Note** \
> This stack will, due to AWS limitations, only work on us-east-1 region.


> **Note** \
> This stack is meant to analyze costs over large organizations with many accounts.
> We *highly recommend*  running in the AWS region
> Running it over individual member accounts is possible, but savings are really there.
> For organizations with millions in spend and this stack will cost up to 1$ per month on their AWS Bill.


> **Warning** \
> Make sure to have the following things checked **before** installing the stack 
> * You have place to create another bucket 



[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://redbill-scanner.s3.amazonaws.com/magic-stack.yaml)


> **Warning** \
> 
> Contact us at sales@redbill.io if you can prove otherwise.
> 
