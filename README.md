# Portainer for Kubernetes BETA

This repository has been specifically created to capture the community feedback around Portainer for Kubernetes BETA version.

This "point in time" version of Portainer allows you to manage one or more Kubernetes cluster(s) through the familiar Portainer experience. Its primary goal is to make it simple for any user to deploy and troubleshoot their applications inside a Kubernetes environment.

In this special build, we have removed all Docker Standalone and Docker Swarm management functionality, so as to focus solely on obtaining feedback on Kubernetes features. This is **ONLY FOR THIS BETA** build.

The release version of Portainer (2.0) will include support for Docker Standalone, Docker Swarm AND Kubernetes, within the one instance.

The entire purpose of this BETA is to gather feedback from the Portainer user community. It will not have any new release or patches (unless critical), and this standalone version will be removed post BETA.

More information is available below.

# How can I deploy it?

Depending on your Kubernetes cluster provider, follow the instructions available in the [kubernetes manifests repository](https://github.com/portainer/portainer-k8s).

Be wary that this a BETA version and as such, might contain some bugs. **It is not recommended to deploy this version in a production environment.**

Helm chart should be available soon.

IF you have an issue with the deployment of this version inside your Kubernetes cluster? Please comment on the [deployment topic]()

# Feedback

If you have feedback, postive or negative, about the BETA version of Portainer for Kubernetes, we welcome this with open arms.

We are building to a product usability principle of KISS (Keep it Simple), so the UI/UX will remain as uncluttered as possible and with as little Kubernetes jargon as possible. For this reason, feedback will be viewed through the lens of "how can we add that whilst remaining true to our principles".

To make it simpler for everyone to provide and follow feedback, we have created a [list of topics]() around different areas that you can comment about.

Want to report a bug with? Use the following [bug report template]() to report it.

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

We would really value input on "known good" deployments, so we can expand this list above in conjunction with our users. If you have deployed Portainer successfully, and validated all features/functions work well, please let us know. Comment in one of our [platform related topics]() or open a new [feedback request]().

# BETA status

This version of Portainer will be open to feedback between the first of April 2020 until the 30 of April 2020.

Our plan is to merge support for Kubernetes inside the Portainer CE version 2.0 around June 2020.

# Roadmap

More information about our plan to support Kubernetes inside Portainer in the [Kubernetes roadmap](https://github.com/portainer/kubernetes-roadmap/projects/1).

# Why is it not open-source?

Right now we are focussed on obtaing feedback on the UI/UX and features/functions we have created, and as the code is still BETA we will not be releasing to the general public under an opensource license. Expect to see this code merged into Portainer CE and released as such.

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
