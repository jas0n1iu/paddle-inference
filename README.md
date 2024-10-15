# PaddleOCR Inference on Amazon SageMaker

This repository contains a Jupyter Notebook that demonstrates how to deploy and perform inference with a PaddleOCR model on Amazon SageMaker. The notebook covers the following steps:

1. **Building and Pushing a Docker Image**: The notebook starts by building a Docker image for the PaddleOCR model and pushing it to Amazon Elastic Container Registry (ECR).
2. **Deploying the Model**: After building the Docker image, the notebook creates a SageMaker Model from the training output and an Endpoint Configuration.
3. **Creating an Endpoint**: The notebook then creates a SageMaker Endpoint using the Endpoint Configuration. This step takes around 9-11 minutes to complete.
4. **Performing Inference**: Once the Endpoint is created, the notebook demonstrates how to perform inference on a sample image using the deployed PaddleOCR model.
5. **Cleaning Up**: Finally, the notebook provides instructions on how to delete the Endpoint, Endpoint Configuration, and Model to clean up the resources.

## Prerequisites

Before running the notebook, ensure that you have the following prerequisites:

- An AWS account with appropriate permissions to create and manage SageMaker resources.
- The AWS CLI installed and configured on your local machine.
- A sample image file (e.g., `1.jpg`) in the `./input/data` directory for inference.

## Usage

1. Clone this repository to your local machine.
2. Open the Jupyter Notebook (`PaddleOCR_Inference.ipynb`) in your preferred environment (e.g., SageMaker Notebook Instance, local Jupyter Notebook).
3. Follow the instructions in the notebook to build the Docker image, deploy the model, create an Endpoint, perform inference, and clean up resources.

## Contributing

Contributions to this repository are welcome. If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](http://private-llm-qa-bot-1466657168.us-west-2.elb.amazonaws.com/LICENSE).

## Acknowledgments

This notebook was created using the Amazon SageMaker Python SDK and the PaddleOCR library. Special thanks to the developers of these projects for their contributions.