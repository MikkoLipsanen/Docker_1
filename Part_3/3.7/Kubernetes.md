# Kubernetes

## When and why to use Kubernetes?

A container orchestration platform like Kubernetes becomes especially handy in cases where there is a need 
to manage a network of containers and multiple hosts. Kubernetes makes it possible to automate to a large 
extent the coordination of a large number of containers which are spread across clusters of servers. 
While in many cases this could also be done manually, an orchestration platform can help to save a huge 
amount of resources.

## What does  Kubernetes offer?

Some of the services offered by Kubernetes are:
* Load balancing to guarantee reliable deployment
* Efficient use of resources based on limits set by the user
* A mechanism that the applications can use to communicate with each other
* Constant monitoring of the network and fault fixing when needed (self-healing system)

## Other similar tools

Even though Kubernetes is currently the most popular container orchestration platform, it is not the only 
player in the market. 

Docker offers it’s own orchestration tool,** Docker Swarm**, that has much of the same functionalities as Kubernetes. 
For users already familiar with Docker, Docker Swarm has the advantage of familiarity: for example most of the Docker 
CLI commands also work with Docker Swarm. Compared to Kubernetes, Swarm is also lighter and easier to install and deploy. 
On the other hand it lacks some of the functionality and advantages of large community that Kubernetes has (for example 
many cloud providers offer Kubernetes as a service)

Third major container orchestration tool in the market is **Apache Mesos**. Compared to Kubernetes it is quite a complex 
platform that is best suitable for very large distributed clusters: it is being used by Twitter and Uber, among others. 
Mesos can be also used to handle non-containerized workloads, and it has specific frameworks (like Marathon) that are used 
for container orchestration.
