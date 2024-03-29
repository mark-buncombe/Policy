### Production Access and Secrets Management

Buncombe County leverages a combination of [na credentials
store](https://support.cloudbees.com/hc/en-us/articles/203802500-Injecting-Secrets-into-na-Build-Jobs),
[credstash](https://github.com/fugue/credstash), and [Amazon EC2 Systems Manager
Parameter
Store](https://aws.amazon.com/blogs/mt/the-right-way-to-store-secrets-using-parameter-store/)
to securely store production secrets.  Secrets are always encrypted; access to
secrets is always controlled and audited.

Details and usage are documented on the Buncombe County Engineering Wiki.