# Deployment

## :pushpin: Description

This folder contains coding demonstration and exercises on how to create a Deployment using a Kubernetes configuration file (YAML)

## :rocket: Execution

Follow this steps when executing this project

1.  :open_file_folder: Clone and explore the repository.

    ```bash
    # clone through ssh
    git clone git@github.com:MHSoquiat/kubernetes-practice.git

    #clone through http
    git clone https://github.com/MHSoquiat/kubernetes-practice.git

    # change directory
    cd kubernetes-practice/5-services

    # list and check the files
    ls
    # services.yaml   - kubernetes configuration file for services
    # README.md       - contains execution instructions
    ```

2. :gear: Pre-requisites: Make sure that there is a deployment running in your device.

    :point_right: Check this one out [Go to Deployment Folder](../3-deployment/)

    > Once done in the deployment, you can now proceed to the next step

3.  :hammer: Build and validate the service configuration file by executing the following commands

    ```bash
    # create deployment
    kubectl create -f services.yaml

    # check whether service is created successfully 
    kubectl get svc
    ```

4. :globe_with_meridians: Access your URL by executing this minikube command:

    ```bash
    # If you are using minikube, you can access the url by this command:
    minikube service myapp-service --url
    ```

:white_check_mark: Here is what the output would look like:

![Expected Output](../5-services/outputs/image.png)

## :bookmark_tabs: Key Takeaways
- Gain hands-on experience in creating and managing Kubernetes deployments and services.

- Understand how to validate configurations and troubleshoot potential issues.

- Learn how to expose applications to the outside world using Kubernetes services.

- Strengthen your skills in container orchestration and cloud-native development.

Working on this repository highlights the importance of networking in Kubernetes and how Services ensure reliable communication between application components. It also demonstrates the practicality of combining theoretical concepts with hands-on practice, making Kubernetes less intimidating and more approachable. The step-by-step exercises allow learners to gradually build confidence, not just in writing YAML files, but also in understanding how Kubernetes orchestrates applications at scale.