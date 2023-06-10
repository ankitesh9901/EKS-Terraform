# Provisioning an EKS Cluster with Terraform

This repository contains Terraform code to provision an Amazon Elastic Kubernetes Service (EKS) cluster in the EU (London) region using the AWS provider.

## Prerequisites

Before you begin, ensure that you have the following prerequisites:

- AWS CLI installed and configured with appropriate credentials.
- Terraform installed on your local machine.


## To connect to the EKS cluster using the kubectl command, run the following command:

bash

    aws eks update-kubeconfig --region <region> --name <cluster_name>

    Replace <region> with the AWS region where the cluster is deployed (e.g., eu-west-2), and <cluster_name> with the name of your EKS cluster.

    You can now use kubectl commands to interact with your EKS cluster.

## Cleanup

To destroy the provisioned EKS cluster and associated resources, run the following command:

bash

terraform destroy

Confirm the destruction by typing yes when prompted.

## Contributing

Contributions are welcome! If you find any issues or want to extend the functionality, feel free to open a pull request.

## License

### This project is licensed under the MIT License.
