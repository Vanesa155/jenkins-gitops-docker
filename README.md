# Jenkins GitOps Docker Repository

This project shows how to build a simple Python Flask app and automate its deployment using Jenkins, Docker, and ArgoCD with a GitOps approach. The Dockerfile containerizes the app, and the Jenkinsfile defines steps to build, push the image to Docker Hub, and update the Kubernetes manifest.

A small fix was added to the Jenkinsfile to support Docker inside Jenkins by setting two environment variables. Jenkins connects to GitHub and Docker Hub using stored credentials, builds the image, and updates the deployment file in a GitOps repo.

ArgoCD then watches that GitOps repo and applies the new deployment automatically in Kubernetes. You can expose the app via Minikube to test it.

This setup shows a full CI/CD flow with modern DevOps tools.


Welcome to the Jenkins GitOps Docker repository! This repository contains the Dockerfile, Jenkinsfile, and application code necessary for building and deploying a Flask application using Jenkins in a GitOps workflow.

## Overview

In this repository, you'll find the following files:

- `Dockerfile`: Defines the Docker image for the Flask application.
- `Jenkinsfile`: Defines the Jenkins pipeline stages for building, testing, and pushing the Docker image.
- `app.py`: Contains the code for a simple Flask application.
- `requirements.txt`: Specifies the Python dependencies required by the Flask application.

## Getting Started

To get started with building and deploying the Flask application using Jenkins and Docker, follow these steps:

1. **Clone the Repository:** Clone this repository to your local machine.

2. **Configure Jenkins:** Set up Jenkins to trigger pipelines based on changes to this repository. Ensure that Jenkins is installed and configured properly.

3. **Configure Docker Hub Credentials:** Add your Docker Hub credentials to Jenkins to allow pushing the Docker image to Docker Hub. Refer to Jenkins documentation for instructions on adding credentials.

4. **Update Jenkins Pipeline:** Customize the Jenkinsfile if necessary to match your Jenkins configuration and requirements.

5. **Commit Changes:** Once you've configured Jenkins and updated the pipeline, commit the changes to this repository.

6. **Monitor Build:** Jenkins will automatically detect changes in this repository and trigger pipeline jobs to build and push the Docker image. Monitor the pipeline execution and Docker image build status in Jenkins.

## Additional Resources

For more information on setting up a complete CI/CD pipeline with Jenkins, Docker, Kubernetes, and ArgoCD, check out our comprehensive guide on Medium:
[Building a Robust CI/CD Pipeline with Jenkins, Docker, Kubernetes, and ArgoCD](https://medium.com/@sameeradissanayaka/building-a-robust-ci-cd-pipeline-with-jenkins-docker-kubernetes-and-argocd-bdcc15a31a2f)

## Contributions

Contributions to this repository are welcome! If you have any suggestions, improvements, or bug fixes, feel free to open an issue or submit a pull request.

## License

This repository is licensed under the [MIT License](LICENSE).


![Captura de pantalla 2025-05-13 231059](https://github.com/user-attachments/assets/f20bda59-9292-4565-b1c2-c5892262b0f1)

![Captura de pantalla 2025-05-14 130622](https://github.com/user-attachments/assets/55e7cf87-03bf-4ec6-8707-92390afe8505)

![Captura de pantalla 2025-05-14 150544](https://github.com/user-attachments/assets/d010844e-1640-4f38-9508-b88b5e6070b1)

![Captura de pantalla 2025-05-14 152631](https://github.com/user-attachments/assets/d667c563-fc02-4024-bdcc-c93e85f08fce)

![Captura de pantalla 2025-05-14 152648](https://github.com/user-attachments/assets/00b80962-42e1-4ca3-950c-0b515c5556a4)

![Captura de pantalla 2025-05-14 152733](https://github.com/user-attachments/assets/6197e388-c42e-4fe1-a3e2-76b5a1bdd647)

![Captura de pantalla 2025-05-14 155625](https://github.com/user-attachments/assets/df41cba8-7a5b-4de9-9da9-472ea5684036)

![Captura de pantalla 2025-05-14 170713](https://github.com/user-attachments/assets/41f7e35e-aa60-41fc-be62-48c3f67640b7)

![Captura de pantalla 2025-05-14 170736](https://github.com/user-attachments/assets/cd08912b-3869-4831-927a-8ee20eadbde8)

## <b> Autora </b>

+ [Gloria Vanesa](https://github.com/Vanesa155 "Vanesa V.")

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
