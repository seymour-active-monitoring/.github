<a href="https://seymour-active-monitoring.github.io/seymour-website/"><img width="258" alt="seymour_drkblue_text" src="https://user-images.githubusercontent.com/30358327/185293218-a4e1439f-d9bc-4eb3-b4e0-48e937a5dfa6.png"></a>


  ## About

Seymour offers open-source, easy-to-configure active monitoring, allowing users test their API endpoints continuously from globally distributed locations. Seymour measures the availability, latency and correctness of API endpoint responses, and sends alerts when these don't meet expectations. 

<img width="1060" alt="Screen Shot 2022-08-17 at 3 59 02 PM" src="https://user-images.githubusercontent.com/30358327/185258138-8883f9b4-37b9-4a41-9af5-900b0a3dc2fb.png">


## Why we built Seymour

We built Seymour to enable rapid detection of issues in production before they impact user experience.

## Get started

Seymour's infrastructure is easily deployed on your AWS account with [two CLI commands](https://github.com/seymour-active-monitoring/infra-setup).

## Repos

1. [tests-ui](https://github.com/seymour-active-monitoring/tests-ui) provides a simple interface for configuring tests and viewing test run results
2. [tests-crud](https://github.com/seymour-active-monitoring/tests-crud) manages test configuration CRUD operations, result aggregation and communicates with AWS EventBridge through the AWS SDK
3. [test-route-packager](https://github.com/seymour-active-monitoring/test-route-packager) is a Lambda responsbile for packaging data for distribute to remote regions
4. [test-runner](https://github.com/seymour-active-monitoring/test-runner) is a Lambda responsible for executing the test configuration-defined API call and assessing the response
5. [test-result-writer](https://github.com/seymour-active-monitoring/test-result-writer) is a Lambda responsible for persisting test results, and, for failed tests, triggering the `test-alerts` Lambda
6. [test-alerts](https://github.com/seymour-active-monitoring/test-alerts) is a Lambda responsible for sending notifications through various channels (email, slack, discord)

## Learn More
Read the [case study](https://seymour-active-monitoring.github.io/) to learn more.

