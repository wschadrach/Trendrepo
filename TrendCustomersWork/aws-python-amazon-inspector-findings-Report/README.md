# Inspector vulnerability report.

This script will deploy a lambda function that will run a report of vulnerabilities from EC2 instances that Amazon Inspector detects and match them against Trend Micro IPS rules.

Click the below to launch the CloudFormation template.

[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=c1ws-inspector-findings-protection&templateURL=https://cloudone-community.s3.us-east-1.amazonaws.com/latest/Workload-Security/Integration/aws-python-amazon-inspector-integration/templates/c1ws-inspector-findings-template.yaml) 



## Prerequisites

1. Valid [Cloud One account](https://cloudone.trendmicro.com/trial) with current subscription to [Workload Security](https://aws.amazon.com/marketplace/pp/prodview-g232pyu6l55l4).

2. You must enable [Amazon Inspector](https://docs.aws.amazon.com/inspector/latest/user/getting_started_tutorial.html) in your AWS account.

3. You need to [verify the email](https://docs.aws.amazon.com/ses/latest/dg/creating-identities.html) you want to send the report (both the vulnerability report and the auto assigned report) to, in Amazon SES.

4. Generate the [API Key](https://cloudone.trendmicro.com/docs/identity-and-account-management/c1-api-key/) from Cloud One.

   > **NOTE:**  You need to verify the email you want the report to send to in the AWS console with SES service

6. For more information about cron expression [Click Here](https://www.designcise.com/web/tutorial/how-to-fix-parameter-scheduleexpression-is-not-valid-serverless-error)
