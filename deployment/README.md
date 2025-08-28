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
    cd kubernetes-practice/deployment

    # list and check the files
    ls
    # deployment.yaml   - kubernetes configuration file for deployment
    # README.md         - contains execution instructions
    ```

2.  Build and validate the deployment configuration file by executing the following commands

    ```bash
    # create deployment
    kubectl create -f deployment.yaml

    # check whether deployment is created successfully 
    kubectl get deployment

    # check the pods created under the replicaset
    kubectl get pods

    #check the replicaset under the deployment
    kubectl get replicaset
    ```

## :bookmark_tabs: Key Takeaways
- Defined and deployed a Kubernetes Deployment using YAML.

- Verified Deployment, Pods, and ReplicaSet creation with kubectl.

- Observed how Deployments automatically manage ReplicaSets and Pods.

- Built a foundation for exploring rolling updates, rollbacks, and scaling.

This project highlights the importance of Deployments in Kubernetes as a powerful abstraction for managing workloads. Deployments not only simplify Pod and ReplicaSet management but also provide advanced capabilities like rolling updates, rollback strategies, and scaling. By practicing with this project, learners strengthen their understanding of reliable, production-ready workload management in Kubernetes, which is essential for building robust and scalable cloud-native applications.
