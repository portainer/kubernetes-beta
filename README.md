# Portainer for Kubernetes BETA

This repository is dedicated to user feedback around the Portainer for Kubernetes BETA version.

# How can I deploy it?

Depending on your Kubernetes cluster provider, follow the instructions available in the [kubernetes manifests repository](https://github.com/portainer/portainer-k8s).

Be wary that this a Beta version and as such, might contain some bugs. It is not recommended to deploy this version in a production environment.

Helm chart should be available soon.

# Feedback

TBD

# Supported platforms and Kubernetes versions

This version of Portainer has been succesfully deployed inside the following cloud provider Kubernetes clusters:

* DigitalOcean
* Azure AKS

It has also been succesfully deployed through the following local cluster providers:

* minikube
* kind

Currently tested against the following Kubernetes versions:

* 1.15.7
* 1.16.2
* 1.17.4

**NOTE**: This version has not been tested against version 1.18 yet.

Have some feedback regarding the deployment of the Beta version on a specific provider/platform? Have a look at our [platform related topics]() or open a new [feedback request](). 

# Beta status

TBD
Beta available from... to... plan is to...

# Roadmap

More information on our plans to support Kubernetes inside Portainer in the [Kubernetes roadmap](https://github.com/portainer/kubernetes-roadmap/projects/1).

# Why is it not open-source? (rephrase)

TBD
This version of Portainer is closed source...

# TO-DO

- [ ] Issue templates (bug report, feedback/feature request, to be determined)
- [ ] Better README
  - [x] Link to useful documentations/install links etc
  - [ ] Link to bug report
  - [ ] Link to feature request etc
  - [ ] Documentation about the project status (not open-source, image available) Answer to why not open-source?
  - [ ] Supported k8s versions
  - [ ] Supported platforms (linux amd64), requests for other platforms open
- [x] Public roadmap document
