## Query CloudFormation Stacks by Tag

Using the AWS CLI, you can list stacks with associated tags using the `describe-stacks` command with the `--query` flag:

```
aws cloudformation describe-stacks --query 'Stacks[?Tags[?Key == `tagkey` && Value == `tagvalue`]].{StackName: StackName}'
```

Hat tip to [this post](https://stackoverflow.com/questions/62783119/how-do-i-filter-cloudformation-stacks-by-tag-value) and [the documentation](https://docs.aws.amazon.com/cli/latest/reference/cloudformation/describe-stacks.html). 