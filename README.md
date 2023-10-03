# Rust Lambda with SAM

Documentation and example of how to build a rust lambda with SAM.

Why Sam? While `cargo lambda` has features to build and deploy your
lambda chances are that you need some more resources in aws. E.g. Hook
the lambda to an actual trigger in aws, create a role for it, provide
permissions, provide a bucket ... yada yada yada.


All of this is pretty much based on [this talk from Luciano Mammino](https://www.youtube.com/watch?v=He4inXmMZZI)
at Rust Dublin.

## Prerequisites

* [Rust](https://rust-lang.org/)
* [Cargo Lambda](https://www.cargo-lambda.info/)
* [SAM Cli](https://github.com/aws/aws-sam-cli)

### Cargo Lambda

A cargo subcommand that provides the


### SAM

SAM is the Serverless Application Model built by AWS. [SAM Docs](https://docs.aws.amazon.com/serverless-application-model/)

TL;DR:
* Sam is a cli app, that provides the interface to build lambdas and deploy
  AWS Resources
* A Template language to define AWS Resources. Its an extension(?) of the
  CloudFormation specification. E.g. Its much like CloudFormation, plus
  some extra features for serverless.

The [samp-app](./sam-app/) folder is the example creates from `sam init`.



## Resources

* https://github.com/awslabs/aws-lambda-rust-runtime/tree/main/examples
* https://github.com/lmammino/earthquake-notifier/tree/main

There is also: https://github.com/cargo-lambda/cargo-lambda-cdk but thats
for another day. :p
