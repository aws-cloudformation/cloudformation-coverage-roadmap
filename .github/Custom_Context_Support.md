Name of Resource:
Custom Context

Issue #: 174612619200828 

Description of changes:
Looking for CLI or CFN support for QueryEditorv2's Amazon Q Custom Context Feature. 

Currently based on Doc, a Custom Context json file can only be submitted through QueryEditorv2's 'Amazon Q generative SQL settings
(admin only)' --> 'upload Custom Context'. A Policy with sqlworkbench:UpdateAccountQSqlSettings must be attached to the users IAM role to access this settings page. 

This is somewhat limiting having to go through the console for both security and CI/CD codepipeline workflows. 
Ideally we would like to limit human QueryEditorv2 admin access. 
We would like to be able to develop a CodePipeline that could either submit a cloudformation template that would upload these Custom Context json files, or create a custom lambda/workflow to upload Custom Context json files via CLI. 

Reference Files:
https://docs.aws.amazon.com/redshift/latest/mgmt/query-editor-v2-generative-ai.html#query-editor-v2-generative-custom-context

By submitting this pull request, I confirm that you can use, modify, copy, and redistribute this contribution, under the terms of your choice.
