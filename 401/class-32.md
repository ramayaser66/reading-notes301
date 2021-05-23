
# Serverless 

![](https://www.xenonstack.com/images/blog/2020/03/aws-serverless-computing-xenonstack.png)
a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers.

using serverless with an application allows it to run in stateless compute containers that are event-triggered, may last for one invocation, and fully managed by the cloud provider. 

Note:
reduced cost is one of the advantages for serverless, 
 The cost model of Serverless is execution-based
 Pricing is based on the number of executions rather than pre-purchased compute capacity 

 You’re allotted a certain number of seconds of use that varies with the amount of memory you require.

**Serverless applications** `--->` are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls
`(Functions as a Service).`


## cloud services:

 - AWS Lambda
- Google Cloud Functions
- Azure Functions
- IBM OpenWhisk
- Alibaba Function Compute
- Iron Functions
- Auth0 Webtask
- Oracle Fn Project
- Kubeless 

## Traditional vs. Serverless Architecture

whene you use servers 
 you'll need  to patch, update, and continuously look after  due to all the  errors. 

 Serverless
  underlying servers are not managed by you, the responsibility falls on the Cloud vendors.

  ## Networking 

  one of the disadvantages of Serverless is 
  Serverless functions are accessed only as private APIs. To access these you must set up an API Gateway.This means you cannot directly access them through the usual IP.

  ## 3rd Party Dependencies 
   another disadvantage: 
   Without system-level access, you must package these dependencies into the application itself.


## Environments 
one of the advantages: 
 you no longer need to set up dev, staging, and production machines. Eventually you’d lose count of all the environments, at some point.

 ## Timeout 
 there’s a hard 300-second timeout limit. Too complex or long-running functions aren’t good for Serverless, but having a hard timeout makes it impossible to perform certain tasks
  A hard limit on this time makes Serverless unusable for applications that have variable execution times, and for certain services which require information from an external source

  ## Scale

 The scaling process for Serverless is automatic and seamless
 but you will face trouble with the control 
 which will make it difficult not to be able to address and mitigate errors related to new Serverless instances.
 

 ## AWS Amplify 

 a set of tools and services that can be used together or on their own, to help front-end web and mobile developers build scalable full stack applications

 It supports popular web frameworks including JavaScript, React, Angular, Vue, Next.js, and mobile platforms including Android, iOS, React Native, Ionic, Flutter. Get to market faster with AWS Amplify.


 
 ## Benefits

 - Configure backends fast 
 - Seamlessly connect frontends
 - Deploy in a few clicks
 - Easily manage content 

 ## Features & Tools 

  1. Develop
  - Authentication
  - API (GraphQL, REST)
  - Storage
  - Interactions
  - PubSub
  - DataStore

(etc ... )


2. Deliver
- Managed Hosting
- CI/CD 
- PR Previews 
- Monitoring
- Custom Domains 

3. Manage 

- Manage Users 
- Manage Content 



