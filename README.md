# Repository Gathering Custom CloudFormation Templates to Create Stacks on AWS

They are grouped according to the services that are spanned by the template Resources:

- `vpc/`: template to create a custom VPC, subnets, an internet gateway, routes, route tables and associations.
- `elastic-beanstalk/`: templates to spin up Elastic Beanstalk applications and environments in a custom VPC by pulling Docker images hosted on ECR or DockerHub.
- `EB-from-private-ECR/`: template that adds the permissions required deploy an EB application by pulling a Docker image from a private ECR registry.
- `EB-with-RDS/`: template to create and couple a PostgreSQL database hosted on RDS with the Elastic Beanstalk application.
- `elastic-container-service/`: templates to spin up an ECS cluster, service and a task in a custom VPC by pulling a Docker image.
- `EB-with-ECS/`: templates to combine the Elastic Beanstalk app with the ECS cluster, let the EC2 instances from both services communicate. In particular, spinning up a fleet of Flask apps running behing an Auto-Scaling Group in EB that need to have a Redis cache running independently to synchronize their sessions.
