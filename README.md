# Serverless Docker Image

Docker image with the following installations:
* Node version 6.11.0
* Latest Yarn package manager
* Serverless framework version 1.15.2

This Docker image was built for the purpose of running serverless commands in the build pipeline. 
You can run serverless commands by executing something like:
`docker run -v $(pwd):/opt/app -e AWS_DEFAULT_REGION -e AWS_ACCESS_KEY_ID -e AWS_SECRET_ACCESS_KEY andrewoh531/docker-serverless serverless deploy`