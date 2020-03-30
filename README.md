# Portainer for Kubernetes BETA

This repository is dedicated to community feedback around the Portainer for Kubernetes BETA version.

This version of Portainer allows you to manage one or multiple Kubernetes cluster through the familiar Portainer experience. Its primary goal is to make it simpler for any user to deploy and troubleshoot their applications inside a Kubernetes environment.

The entire purpose of this version is to gather feedback from the Portainer user community. It will not have any new release or patch (unless critical). More information available in the BETA status section below.

# How can I deploy it?

Depending on your Kubernetes cluster provider, follow the instructions available in the [kubernetes manifests repository](https://github.com/portainer/portainer-k8s).

Be wary that this a BETA version and as such, might contain some bugs. **It is not recommended to deploy this version in a production environment.**

Helm chart should be available soon.

# Feedback

Have some feedback about the BETA version of Portainer for Kubernetes? We're welcoming all the feedback regarding everything Portainer and Kubernetes.

To make it simpler for everyone to provide and follow feedback, we have created a [list of topics]() around different areas that you can comment about.

Want to report a bug with? Use the following [bug report template] to report it.

Would you like to report a feature/enhancement request and did not found any topic to comment in? Use the [following enhancement request template]().

We also have a generic [feedback template]() for any feedback that would not fit into the categories specified above.

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

**NOTE**: This version has not been tested against Kubernetes 1.18 yet.

Have some feedback regarding the deployment of the BETA version on a specific provider/platform? Have succesfully deployed the BETA version inside a specific cluster provider? Comment in one of our [platform related topics]() or open a new [feedback request]().

# BETA status

This version of Portainer will be open to feedback between the first of April 2020 until the 30 of April 2020.

Our plan is to merge support for Kubernetes inside the Portainer CE version around June 2020 to offer support for Docker Swarm, Docker standalone and Kubernetes in the same Portainer version.

# Roadmap

More information about our plan to support Kubernetes inside Portainer in the [Kubernetes roadmap](https://github.com/portainer/kubernetes-roadmap/projects/1).

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
  - [x] Supported k8s versions
  - [x] Supported platforms (linux amd64), requests for other platforms open
- [x] Public roadmap document
