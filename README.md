# Hot Reloading Spring Application Configuration

This repository demonstrates how to hot reload configuration for a Spring application using Kubernetes and AWS. The examples are split into two branches, each showcasing a different approach.

## Video Overview

For a visual walkthrough, watch the file `walkthrough.mp4` stored in this repository.

## Approaches

### 1. Spring Cloud Kubernetes Configuration Watcher

**Branch:** `watcher`

This approach utilizes the Spring Cloud Kubernetes Configuration Watcher to dynamically reload configuration changes. This requires specific Kubernetes permissions to function correctly.

- **Kubernetes Permissions:** Refer to the `k8s` folder for more details on the necessary permissions.
- **Documentation:** For a detailed explanation of how the watcher works, refer to the [Spring Cloud Kubernetes Configuration Watcher documentation](https://docs.spring.io/spring-cloud-kubernetes/reference/spring-cloud-kubernetes-configuration-watcher.html).

### 2. AWS Parameter Store

**Branch:** `parameter-store`

This approach uses AWS Parameter Store to manage and reload configuration properties. You will need to set up IAM credentials, either through environment variables or an IAM role.

- **IAM Credentials:** Set up IAM credentials using environment variables or an IAM role.
- **Documentation:** For more information, refer to the [AWS Spring Cloud documentation](https://github.com/awspring/spring-cloud-aws/tree/main/spring-cloud-aws-samples).

## Getting Started

To get started with either approach, switch to the respective branch. 

```bash
# For Kubernetes Configuration Watcher
git checkout watcher

# For AWS Parameter Store
git checkout parameter-store
