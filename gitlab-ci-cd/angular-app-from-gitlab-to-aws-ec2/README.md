# Angular app from gitlab to aws S3 


## Introduction

dans cet article de blog nous allons apprendre étapes apres étapes comment  mettre en place un circuit de déploiement d'appliactions SPA angular  depuis une source gitlab  sur AWS S3

### Overview of Angular, AWS, and GitLab CI/CD
(Continuous Integration/Continuous Deployment) are three distinct but often used together technologies in modern web development. Let's provide an overview of each:

**1- Angular**
 - **What is it?** Angular is a popular open-source web application framework maintained by Google. It is used for building dynamic, single-page web applications (SPAs) and offers a structured approach to web development.
- **Key Features:**
Component-Based Architecture: Angular applications are built using reusable components.
    - Two-Way Data Binding: Allows for automatic synchronization between the model and the view.
    - Dependency Injection: Promotes modularity and testability by managing dependencies.
    - Routing: Supports client-side routing for building SPAs.
    - TypeScript: Angular is primarily written in TypeScript, a statically typed superset of JavaScript.
- **Use Cases:** 
Angular is suitable for building complex, feature-rich web applications and SPAs

**2 - AWS (Amazon Web Services):** 

- **What is it?** AWS is a comprehensive cloud computing platform provided by Amazon. It offers a wide range of services, including computing power, storage, databases, machine learning, and more, to help organizations scale and deploy applications in the cloud
- **Key Services:**

    - **EC2 (Elastic Compute Cloud):** Provides scalable virtual servers for running applications.
    - **S3 (Simple Storage Service):** Offers scalable object storage for files and data.
    - **Lambda:** Allows you to run code in response to events without provisioning servers.
    - **RDS (Relational Database Service):** Managed relational database service.
    ECS (Elastic Container Service): Orchestrates Docker containers.
- **Use Cases:** AWS can be used for hosting web applications, data storage, machine learning, IoT, and a wide range of other cloud-related tasks.

**3 - GitLab CI/CD:**

- **What is it?** GitLab CI/CD is the continuous integration and continuous deployment platform integrated into GitLab, a web-based Git repository manager. It automates the process of building, testing, and deploying code.
- **Key Features:**
    - **Pipeline Automation:** Allows you to define and automate pipelines for building, testing, and deploying applications.
    - **Version Control:** Integrates tightly with Git repositories for version control.
    - **Container Registry:** Provides a container registry for managing Docker images.
    - **Auto DevOps:** Offers built-in templates for common application types.



### Benefits of using these technologies together

Angular applications can be hosted on AWS, either by deploying them on AWS S3, to EC2 instances or by using AWS Amplify, a service that simplifies web and mobile app hosting. GitLab CI/CD can be used to automate the deployment of Angular applications to AWS, ensuring that changes are tested and deployed continuously. GitLab CI/CD can also be configured to run tests, build Docker containers, and deploy applications to AWS services like Elastic Beanstalk, S3, or ECS.

In summary, Angular is a web development framework, AWS provides cloud infrastructure and services, and GitLab CI/CD is a DevOps tool for automating the software development lifecycle. Together, they enable developers to build, test, and deploy Angular applications in a scalable and efficient manner on the AWS cloud infrastructure.

## Setting Up the Environment

### Creating an AWS account
### Configuring the AWS services
a - create S3 bucket and off  ``` Block all public access  ```
b - change  bucket policy 
c - activate acl 

d - create user
e - generate credential  (acces key and secret key)
f - create gitlab repository
g - save varilable key on gitlab varialble
  
### Setting up the GitLab CI/CD pipeline
a - write deployment file
## Deploying the Application

### Building the application
### Testing the application
### Deploying the application to AWS

## Conclusion

#### Summary of deploying an Angular application to AWS with GitLab CI/CD
#### Benefits of using this combination of technologies
