# Booking System CloudFormation Stack Template

![AWS Architecture](./assets/aws-architecture.png)

- `network.yaml` - creates VPC with 2 public and private subnets each in 2 availability zones, an elastic load balancer and internet gateway
- `service.yaml` - deploys docker containers on Fargate task, which autoscales on demand
- `database.yml` - creates a single RDS MySQL instance into the 2 private subnets