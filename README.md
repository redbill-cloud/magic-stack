# Redbill Scanner - Magic Stack


How does the Magic Stack *work*?

You click a button, and a few days later, RedBill gets an email with the amount you can save across your entire AWS organization.
We contact you and explain the exact actions you need to take to realize the savings. You can realize these recommendations within hours.

[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/review?templateURL=https://redbill-scanner.s3.amazonaws.com/magic-stack.yaml)

The recommended actions are purely financial, meaning the fixing part is easy and:
* No risk of downtime to your resources, applications and systems
* No unexpected outages due to configuration changes
* No complexity of changing hundreds or thousands of resources
* The stack does not require and Trusted connections, a simple AWS SNS message is sent with a short savings report.
* The analysis is free - save the up to a few USD in large enterprise Accounts

> **Warning** \
> Make sure to have the following things checked **before** installing the stack
> * You are logged in into your management account (master payer) (*Recommended*)
> * You have place to create another bucket, check this by accessing S3 bucket quota (*Required*)
> * You have less than 10 Cost and Usage reports within that account (*Required*)


### Transparency

Redbill Magic Stack does not require any access to your account in the initial Scan. 
The Scan outputs potential savings and sends the number to an SNS topic in RedBill's AWS Account. 
We are sure there are easy savings to be made before we even contact you.

All the code is in the stack - so you can read all the code that executes on your account.  It's published as open source in this repository and uploaded to an s3 bucket, from where AWS Cloudfromation can reach it.



You can delete the stack at *any time* with no consequences.

> **Note** \
> This stack will, due to AWS limitations, only work on us-east-1 region.

> **Warning** \
> For organizations with hundreds of accounts and millions in spend and this stack will cost up to $5 per month on their AWS Bill.
> Redbill tags all the resources it creates and uses, so it's 100% transparent on the resources it consumes. 
> Using the following tags you can view the costs transparently in your Cost Explorer: 
> * TagKey: `magic-stack`
> * Tag value `infra` \
> Contact us at sales@redbill.io if you have any questions. 


> **Note** \
> This stack can analyze costs over large organizations with many hundreds of accounts.
> We *highly recommend*  running in the AWS management account for biggest gains, since the stack is built to analyze all accounts,
> and some savings can be only applied efficiently at the Organizational level.

