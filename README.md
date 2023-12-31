# Jenkins-CI-CD-Pipeline-for-Portfolio
## Overview
This project utilizes a CI/CD pipeline to automate the deployment of my personal portfolio. It integrates various tools and services, including GitHub, Jenkins, Ansible, Docker, AWS EC2, and AWS Route53.

![Jenkins CI_CD Portfolio drawio](https://github.com/iamdhrutipatel/Jenkins-CI-CD-Pipeline-for-Portfolio/assets/58872872/0cd5b9f7-4f42-455b-9087-224f54cbf20f)

## Architecture
The following components make up the pipeline:

- **GitHub:** Hosts the source code and utilizes webhooks to trigger the pipeline on a push event.
- **Jenkins:** Orchestrates the pipeline, running jobs to build, test, and deploy the application.
- **Ansible:** Configures the necessary environments and dependencies.
- **Docker:** Packages the application into a container for consistent deployment.
- **AWS EC2:** Hosts the running containers in a scalable and reliable cloud environment.
- **AWS Route53:** Manages DNS for the portfolio, routing traffic to the appropriate instance.

## Workflow
1. **Code Push:** Developers push code to the GitHub repository.
2. **Webhooks:** GitHub webhooks automatically notify Jenkins to start a new build.
3. **Build and Test:** Jenkins retrieves the latest code and executes defined jobs to build and test the application.
4. **Containerization:** If tests pass, Jenkins uses Ansible to build a Docker container.
5. **Deployment:** The Docker container is deployed to AWS EC2 instances.
6. **Routing Traffic:** AWS Route53 routes incoming traffic to the docker instance.

## License

This project is licensed under the [MIT License](LICENSE).

## Developer 
[Dhruti Patel](https://github.com/iamdhrutipatel) 
