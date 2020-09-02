# Important notice

This repository has been archived.

Portainer 2.0 includes support for Kubernetes, head to https://www.portainer.io/installation/ for more details about how to install it.

# Portainer for Kubernetes BETA

This repository has been specifically created to capture the community feedback around Portainer for Kubernetes BETA version.

This "point in time" version of Portainer allows you to manage one or more Kubernetes cluster(s) through the familiar Portainer experience. It's primary goal is to make it simple for any user to deploy and troubleshoot their applications inside a Kubernetes environment.

In this special build, we have removed all Docker Standalone and Docker Swarm management functionality, so as to focus solely on obtaining feedback on Kubernetes features. This is **ONLY FOR THIS BETA** build.

The release version of Portainer CE (2.0) will include support for Docker Standalone, Docker Swarm AND Kubernetes, within the one instance.

The entire purpose of this BETA is to gather feedback from the Portainer user community. It will not have any new releases or patches (unless critical), and this BETA version will be removed post BETA.

Be sure to read the FAQ section below for current known limitations and other sections for more information.

# How can I deploy it?

Depending on your Kubernetes cluster provider, follow the instructions available in the [Kubernetes manifests repository](https://github.com/portainer/portainer-k8s).

Be wary that this a BETA version and as such, might contain some bugs. **It is not recommended to deploy this version in a production environment.**

IF you have an issue with the deployment of this version inside your Kubernetes cluster, please comment on the [deployment topic](https://github.com/portainer/kubernetes-beta/issues/1).

# Feedback

If you have feedback, positive or negative about the BETA version of Portainer for Kubernetes we welcome this with open arms.

We are building to a product usability principle of KISS (Keep it Simple, Stupid), so the UX/UI will remain uncluttered with as little Kubernetes jargon as possible. For this reason, feedback will be viewed through the lens of "how can we add that whilst remaining true to our principles".

To make it simpler for everyone to provide and follow feedback, we have created a [list of topics](https://github.com/portainer/kubernetes-beta/issues?q=is%3Aissue+is%3Aopen+%5BTOPIC%5D) around different areas that you can comment about.

* Want to report a bug with this BETA? Use the following [bug report template](https://github.com/portainer/kubernetes-beta/issues/new?template=bug_report.md) to report it.

* Would you like to report a feature/enhancement request and you haven't found any topics to comment in? Use the [following enhancement request template](https://github.com/portainer/kubernetes-beta/issues/new?template=feature_request.md).

* We also have a generic [feedback template](https://github.com/portainer/kubernetes-beta/issues/new?template=custom.md) for any feedback that would not fit into the categories specified above.

You can also [join us on Slack](https://join.slack.com/t/portainer/shared_invite/enQtNDk3ODQ5MjI2MjI4LTcwNGYxMWQ5OGViYWZkNDY2ZjY4YTMwMTgzYmU4YmNiOTU0MDcxYmJjNTIyYmQ0MTM5Y2QwNTg3NzNkMTk5MDg) to discuss it in our #kubernetes-beta channel.  

# Supported platforms and Kubernetes versions

This version of Portainer has been successfully deployed inside the following cloud provider Kubernetes clusters:

* DigitalOcean
* Azure AKS

It has also been successfully deployed through the following local cluster providers:

* minikube
* kind

Currently tested against the following Kubernetes versions:

* 1.15.7
* 1.16.2
* 1.17.4

**NOTE**: This version has not been tested against Kubernetes 1.18 as of yet.

We would really value input on "known good" deployments, so we can expand this list above in conjunction with our users. If you have deployed Portainer successfully and validated all features/functions work well, please let us know.

You can comment in one of our [platform related topics](https://github.com/portainer/kubernetes-beta/issues?q=is%3Aissue+is%3Aopen+%5BTOPIC%5D+label%3Atopic%2Fplatform) or open a new [feedback request](https://github.com/portainer/kubernetes-beta/issues/new?template=custom.md).

# BETA status

This version of Portainer will be open to feedback between the 1st of April 2020 until the 30th of April 2020.

Our plan is to merge support for Kubernetes inside the Portainer CE version 2.0 around June 2020.

# Roadmap

More information about our plan to support Kubernetes inside Portainer in our [Kubernetes roadmap](https://github.com/portainer/kubernetes-roadmap/projects/1).

Feel free to contribute in there too!

# FAQ

## Why do I need to reconfigure Portainer each time it is restarted?

In the BETA, we have not configured Portainer to persist its configuration. This is, in part, to discourage its use in Production environments. However, if you wish to persist the data, you need to manually edit the deployment instructions to persist the `/data` container folder.

## Why am I not seeing all the deployed applications running inside my cluster in the Applications list?

In this current BETA, Applications will only display the following Kubernetes workloads: **Deployments**, **StatefulSets** and **DaemonSets**.

We'll add support for isolated pods in a future version, see https://github.com/portainer/portainer/issues/4011
