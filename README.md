# Tomcat Docker Images

This project builds the extended version of tomcat for a number of linux distributions for arm64 and amd64 architectures.

The images are found at the following locations:

 * [Docker Hub Repository](https://hub.docker.com/repository/docker/truemark/tomcat/general)
 * [Amazon ECR Repository](https://gallery.ecr.aws/truemark/tomcat)


Example Amazon ECR
```bash
aws ecr-public get-login-password --region us-east-1 | docker login --username AWS --password-stdin public.ecr.aws
docker pull public.ecr.aws/truemark/tomcat:8.0.21-temurin-jdk8
```

Example Docker Hub
```bash
docker login -u <<username>> -p <<password>> docker.io
docker pull docker.io/truemark/tomcat:8.0.21-temurin-jdk8
```