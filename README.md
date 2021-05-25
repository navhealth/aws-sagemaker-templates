CloudFormation templates for setting up Amazon SageMaker notebook instances.

## Features

* CloudFormation templates for setting up infrastructure needed to use Amazon SageMaker
  securely in a multi-tenant environment.
* CloudFormation templates that allow users to manage their own Amazon SageMaker
  resources in a secure fashion.

## Usage

### Simple Deployment

```bash
NAME=firstnamelastname make create-sagemaker-notebook-instance
```

### Different Team

```bash
NAME=firstnamelastname DEPLOYMENT_NAME=Engineering make create-sagemaker-notebook-instance
```

### Different Instance Type
Allowed instance types:
* **ml.t3.large**
* ml.t3.xlarge
* ml.t3.2xlarge
* ml.m5.large
* ml.m5.xlarge
* ml.m5.2xlarge
* ml.m5.4xlarge
* ml.m5.12xlarge
* ml.m5.24xlarge


```
NAME=firstnamelastname INSTANCE_TYPE=ml.m5.large make create-sagemaker-notebook-instance
