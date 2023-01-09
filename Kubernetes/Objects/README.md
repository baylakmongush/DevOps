# Kubernetes objects

All objects at Kubernetes are represented by a JSON/YAML file. The file contains the object’s specification. The object’s specification contains the following fields:

* apiVersion - version of the API
* kind - type of the object
* metadata - data that helps to identify the object: name, labels, annotations
* spec - specification of the object
* status - current status of the object

## Namespaces

Namespaces are used to organize objects into groups. Namespaces are used to separate objects in different environments. For example, you can have a namespace for development, a namespace for testing, and a namespace for production. Namespaces are also used to separate objects in different teams. For example, you can have a namespace for the frontend team, a namespace for the backend team, and a namespace for the database team.

Namespaces are not used to separate objects in different projects. For example, you can have a namespace for the frontend project, a namespace for the backend project, and a namespace for the database project.

Namespace prod, dev, and test are created by default. You can create your own namespaces.

## Selectors and labels

Labels are key/value pairs that are attached to objects. Labels are used to identify objects. Labels are used to select objects. Labels are used to organize objects. Labels are used to group objects. Labels are used to filter objects. Labels are used to sort objects. Labels are used to match objects.

Selectors are used to select objects. Selectors are used to filter objects. Selectors are used to sort objects. Selectors are used to match objects.

## Pods

Pods are the smallest deployable units of computing that you can create and manage in Kubernetes. A Pod represents processes running on your cluster.

A Pod encapsulates an application’ container (or, in some cases, multiple containers), storage resources, a unique network IP, and options that govern how the container(s) should run. A Pod represents a unit of deployment: * a single instance of an application in Kubernetes, which might consist of either a single container or a small number of containers that are tightly coupled and that share resources.

A Pod is a Kubernetes abstraction that represents a group of one or more application containers (such as Docker or rkt), and some shared resources for those containers. Those resources include:

* Shared storage, as Volumes
* Networking, as a unique cluster IP address

A Pod models an application-specific “logical host” - it contains one or more application containers which are relatively tightly coupled - in a pre-container world, they would have executed on the same physical or virtual machine.

