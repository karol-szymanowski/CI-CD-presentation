# CI/CD - Jenkins
How to automate app’s testing and deployment using **Jenkinsfile**

## Introduction
The most common source of mistakes and errors in workplace environment is human. 
especially if their work is repeatable. That’s why every task that can be done by a machine should be.  It helps reduce errors greatly and releases human resources that have so far been used to maintain software and gives them more time to improve software.

### What is Continuous Integration?
Continuous integration is continuous testing in a way, which does not affect developers productivity. CI has become common practice among developers. One of the main reasons is it’s relatively low price at a high value.

By integrating regularly, it becomes possible to detect errors, locate and eliminate them more quickly, on the early stage of features development and prevent deployment if there is one.

The main point of continuous integration is to detect errors as early as possible in build process. It uses so called integration machine to “integrate” new feature with mainline code.

### What is Continuous Delivery?
Continuous delivery is closely related to CI term, CD complements CI. CD ensures, that code is ready can be shipped any time. **Requires CI!**

### What is Continuous Deployment (also CD)?
The main purpose of CD is to release every good build to the users.

### Benefits from implementing CI/CD process in projects
A well-designed CI / CD process gives great value to projects. Some of them are obvious, others are not necessary. Here are a few of them that encourage you to put them into your projects.

#### Continuous Integration:
1. Detecting bug in early stage - the earlier bug is detected, the less harm it makes
2. Reduces bug count.
3. The development process becomes more transparent - teams is notifed when build fails and what caused it.
4. Efficient - since whole process is automated, manual testing is reduced.

#### Continuous Delivery & Deployment:
1. Reduce the risk - deployment process may get complicated. It can consist of many steps. The more complicated the process, the greater the probability of human error. By automating this process we can assure, that every deployment will look similar.
2. Painless deployment, happier team - all it needs is approval from the person responsible for project.
3. Reduces costs.
4. Fully automated and transparent process.

## CI/CD process
Diagram of how CI/CD process may look like:

```
code > commit changes > build > unit test > deploy to staging machine > auto tests > deploy to production
```

## How to start
There are many tools and services on the market to implement ci/cd. The most popular ones are:
- Travis CI
- Circle CI
- Jenkins
- TeamCity
- Gitlab CI
- Codeship
- Bamboo

The easiest one to integrate are services like Travis CI or Circle CI. They does not require any servers or complicated configurations to set them up. Tools like Jenkins require a server and configuration can give you a headache but it gives you more freedom in terms of how process will look.

Picking appropriate tool is crucial and will define the whole process later.

### Additional software
Except automation server or service CI/CD process may require additional software to run and/or increase workflow experience:
- Docker
- Kubernates
- PM2
- Virtual machines
- All sorts of communication apps

## Sources
- https://jenkins.io/doc/book/pipeline/jenkinsfile/
- https://martinfowler.com/articles/continuousIntegration.html
- https://www.thoughtworks.com/continuous-integration
- https://css-tricks.com/continuous-integration-continuous-deployment/

