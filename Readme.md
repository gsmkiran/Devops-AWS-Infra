##                                      CICD steps on AWS Cloud infrastructure

# Build the Java Spring Boot HelloWorldMicroservice application. This includes running unit tests.
# Performs a security scan on the code base.
# Created security groups in IAM and ECR.
# The environments are AWS EC2 instances and the script files are imaged in S3 buckets.
# Used cloud formation for configuration management of the cloud infrastructure.
# Build and register a version of the Docker image
# Deploy the docker image to the dev environment
# Run the automated browser tests against the application in the dev environment. The browser tests are written in Python using the Python Selenium Webdriver
# Deploy the docker image to the test environment
# Run the automated browser tests against the application in the test environment
# Pause for confirmation that the new image can be deployed to the prod environment. Allow for some manual tests to be executed before This step times out after some (configurable amount of) time.
# Deploy the image to the prod environment