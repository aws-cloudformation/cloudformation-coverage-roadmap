Name of Resource:
Redshift Data Sharing

Subject
CFN Support for Datasharing
Case ID
174733232100728
Created
2025-05-15T18:05:21.413Z
Case type
Technical

Description of changes:
Looking for cloudformation support for redshift's data sharing. Currently only way to create and grant access to/from clusters is either from redshift cli or from within the cluster itself running sql. 

I feel like this should be supported though redshift CFN. The way im thinking of it would be like a datashare resource with parameters like 'producer cluster' / 'name' / then potentially a resource/parameter that would allow you grant access to other consumer clusters. 

Reference Files:
[https://docs.aws.amazon.com/redshift/latest/mgmt/query-editor-v2-generative-ai.html#query-editor-v2-generative-custom-context](https://docs.aws.amazon.com/cli/latest/reference/redshift/)

https://docs.aws.amazon.com/redshift/latest/dg/datashare-overview.html

By submitting this pull request, I confirm that you can use, modify, copy, and redistribute this contribution, under the terms of your choice.
