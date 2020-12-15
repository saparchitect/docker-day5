docker day 5
------------

Topics

* yaml
* 

yaml
----

YAML Ain't Markup Language is a data serialization language that matches user’s expectations about data. It designed to be human friendly and works perfectly with other programming languages. It is useful to manage data and includes Unicode printable characters.

Understanding YAML is important because almost all container related configuration depends on it. A few examples are:

* Docker Compose
* All Kubernetes configs
* Github Actions
* Gitlab CI

Learn how to use yaml by reviewing the tutorial and typing each example into a yaml to json converter

* [tutorial](https://learnxinyminutes.com/docs/yaml/)
* [yaml to json](https://onlineyamltools.com/convert-yaml-to-json)

Github Actions
--------------

Build an app and utilize Github Actions to create a docker based CI/CD process.
* Create a Github account
* Create a new Github project
* Push a project to the repo that utilizes Github Actions and Docker.
* Create a corresponding repo on DockerHub so Github Actions can push to it
* Add DOCKER_USERNAME and DOCKER_PASSWORD to secrets
* Cut a new release that will trigger the build and push the image
* Fix an build failures and try again