# CI Pipeline

This is a global CI pipeline for the organization. It is designed to be used by other repos. It has the following steps:
* If the repo has a custom docker image, it will build then push to ECR
* If not, it allows you to scan the image you plan on using. For example, in the case of the Trivy Service, it scans `aquasec/trivy:latest`.
