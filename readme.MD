In this , I have included both mysql and backend parts and deployed the application into kubenetes. Also included liveness probe and readiness probes.Screenshots of pod logs and describe pods are mentioned below.

First we need to create the namespace. 

Explanation of mysql yaml file

Labels are used as image tags. Only one replicaset is taken.mysql image is taken to deploy.
A liveness probe checks whether your container is running and healthy. If the liveness probe fails, Kubernetes will automatically restart the container to recover from a failure.
A readiness probe checks whether your container is ready to serve traffic. If the readiness probe fails, Kubernetes will stop sending traffic to the container, but it will not restart the container.

Service also should be created inorder to expose this application to external world.

Services in Kubernetes are essential for communication within and outside of the cluster.
They provide stable networking to Pods and ensure that services are discoverable and accessible.

--
--
--

Backend manifest file output

--
--
--