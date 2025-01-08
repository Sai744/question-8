* In this , I have included both mysql and backend parts and deployed the application into kubenetes.
* Also included liveness probe and readiness probes.
* Screenshots of pod logs and describe pods are mentioned below.

First we need to create the namespace. 

* Explanation of mysql yaml file

Labels are used as image tags. Only one replicaset is taken.mysql image is taken to deploy.
A __liveness probe__ checks whether your container is running and healthy. If the liveness probe fails, Kubernetes will automatically restart the container to recover from a failure.

A __readiness probe__ checks whether your container is ready to serve traffic. If the readiness probe fails, Kubernetes will stop sending traffic to the container, but it will not restart the container.

__Service__ also should be created inorder to expose this application to external world.

Services in Kubernetes are essential for communication within and outside of the cluster.
They provide stable networking to Pods and ensure that services are discoverable and accessible.

<<<<<<< HEAD
__mysql manifest file output__
=======
* output of mysql manifest file
>>>>>>> 74a2466f241ed2901a8ac04f9035146e9f69528e

![31](https://github.com/user-attachments/assets/b4daa735-f265-4852-a901-9d48136af999)

![32](https://github.com/user-attachments/assets/1d94da17-178b-4e0a-90be-df52fd9312ca)

![33](https://github.com/user-attachments/assets/4bf22839-393f-402e-8d7b-d19e1255532f)


__Backend manifest file output__

![34](https://github.com/user-attachments/assets/5b315a89-ab90-4867-8245-465b9ea26753)

![35](https://github.com/user-attachments/assets/d8b07ec8-d6c9-4611-8aa4-3139c3ada1e4)

![36](https://github.com/user-attachments/assets/37af9164-3484-46dc-94c3-92a7e025bb4f)
