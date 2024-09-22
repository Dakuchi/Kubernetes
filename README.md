## deploy applicaion with docker image from private repository AWS ECR

![alt text](image1.png)

- Create Kubernetes secret for ECR
    - ``` kubectl create secret generic my-registry-key --from-file=.dockerconfigjson=/home/jayce/.docker/config.json --type=kubernetes.io/dockerconfigjson ```
    - ``` kubectl get secret ```

    ![alt text](image2.png)

- Create configuration file with created secret key

- Deploy the application

    ![alt text](image4.png)
    
    ![alt text](image5.png)