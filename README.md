docker day 5
------------

Topics

* docker development best practices
* docker trust
* docker image vulnerabilites
* docker scan
* yaml
* github actions

docker development best practices
---------------------------------

The following development patterns have proven to be helpful for people building applications with Docker. 

* [Docker Development Best Practices](https://docs.docker.com/develop/dev-best-practices/)

docker trust
------------

When transferring data among networked systems, trust is a central concern. In particular, when communicating over an untrusted medium such as the internet, it is critical to ensure the integrity and the publisher of all the data a system operates on. You use the Docker Engine to push and pull images (data) to a public or private registry. Content trust gives you the ability to verify both the integrity and the publisher of all the data received from a registry over any channel.

* [Docker Trust](https://docs.docker.com/engine/security/trust/)

docker image vulnerabilities
----------------------------

A new security analysis of the 4 million container images hosted on the Docker Hub repository revealed that more than half contained at least one critical vulnerability.

* [Docker Image Vulnerabilities](https://www.csoonline.com/article/3599454/half-of-all-docker-hub-images-have-at-least-one-critical-vulnerability.html)

docker image scanning
---------------------

Vulnerability scanning for Docker local images runs on Snyk engine, providing users with visibility into the security posture of their local Dockerfiles and local images. Users trigger vulnerability scans through the CLI, and use the CLI to view the scan results. The scanning function creates the list of Common Vulnerabilities and Exposures (CVEs), and provides recommendations for CVE remediations.

* [Docker Scan](https://docs.docker.com/engine/scan/)

yaml
----

YAML Ain't Markup Language is a data serialization language that matches user’s expectations about data. It designed to be human friendly and works perfectly with other programming languages. It is useful to manage data and includes Unicode printable characters.

Understanding YAML is important because almost all container related configuration depends on it. A few examples are:

* Docker Compose
* All Kubernetes configs
* Github actions
* Gitlab CI

Learn how to use yaml by reviewing the tutorial and typing each example into a yaml to json converter

* [tutorial](https://learnxinyminutes.com/docs/yaml/)
* [yaml to json](https://onlineyamltools.com/convert-yaml-to-json)

github actions
--------------

Build an app and utilize Github Actions to create a docker based CI/CD process.

* Create a Github account

* Enable the [Github Container Registry](https://docs.github.com/en/free-pro-team@latest/packages/guides/enabling-improved-container-support#enabling-github-container-registry-for-your-personal-account) feature.

* Create a [PAT (Personal Access Token)](https://docs.github.com/en/free-pro-team@latest/github/authenticating-to-github/creating-a-personal-access-token) make sure it has all package permissions.

* Create a new Github project

* Store your personal pat in a [Github Secret](https://docs.github.com/en/free-pro-team@latest/actions/reference/encrypted-secrets#creating-encrypted-secrets-for-a-repository) called `CR_PAT`

* Push the contents of this repo into that project

* Check the actions tag to see build progress. Fix any build failures. HINT: Make the unit test pass by fixing the code in `sum.go`
