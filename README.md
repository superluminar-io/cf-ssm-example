# cf-ssm-example
Example CF Stack to automate EC2 instance termination via SSM

Creates a [SSM Association](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ssm-association.html)
that stops all EC2 instances with a Tag `$TagName` (default `stopme`) and value `$TagValue` (default `"true"`) 
at `$ExecutionHour` (default 18).