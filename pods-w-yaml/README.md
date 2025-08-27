# Pods with YAML

## :pushpin: Description

This folder contains coding demonstration and exercising on how to create a Pod using a Kubernetes configuration file (YAML)

## :rocket: Execution

Follow this steps when executing this project

1.  :open_file_folder: Clone and explore the repository.

    ```bash
    # clone through ssh
    git clone git@github.com:MHSoquiat/kubernetes-practice.git

    #clone through http
    git clone https://github.com/MHSoquiat/kubernetes-practice.git

    # change directory
    cd kubernetes-practice/pods-w-yaml

    # list and check the files
    ls
    # pods.yaml       - kubernetes configuration file
    # README.md       - contains execution instructions
    ```

2.  Build and validate the pod by executing the following commands

    ```bash
    # create pod
    kubectl apply -f pods.yaml

    # check whether pod is created successfully 
    kubectl get pod

    # to see more details about the pod we just created
    kubectl describe pod nginx
    ```

## :bookmark_tabs: Key Takeaways
- Hands-on practice in defining Pods using YAML.

- Understanding of kubectl commands for creating, inspecting, and validating Pods.

- Experience in declarative Kubernetes resource management.

- Foundation for scaling into advanced objects like ReplicaSets, Deployments, and Services.

Working through this project helps me build confidence in Kubernetes fundamentals by applying declarative configurations instead of imperative commands. It emphasizes best practices in resource definition, verification, and inspection, ensuring readiness for more complex workloads in container orchestration. This exercise forms the basis for advancing into multi-container Pods, deployments, scaling, and service discovery within Kubernetes.
