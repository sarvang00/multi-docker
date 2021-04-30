# multi-docker

### Description
In this project, I have made a multi-docker image that is performing CI/CD using Travis CI.

I have built 4 images: 1 each for server, client, worker and the necessary traffic routing(using nginx).

#### Development Environment Setup
![Image of Development Environment Setup](https://github.com/sarvang00/multi-docker/blob/master/docker-compose-architecture.png)

#### Deployment Setup
We have changes deployment a bit. We will use AWS's RDS Postgres Database for Database and AWS ElastiCache for Redis. Thus, we will also make some minor modifications from the Dev Architecture.

It may be better to have a fully self-controlled environment, but by my analysis, for most of the cases, using a fully-managed service is generally better.

![Image of Deployment Setup](https://github.com/sarvang00/multi-docker/blob/master/prod-architecture.png)
