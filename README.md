CodeShip Demo - Building Java project with Jenkinsfile Runner
====

[![Codeship Status for oleg-nenashev/codeship-jfr-java-maven-demo](https://app.codeship.com/projects/43076db0-e6aa-0138-3875-02cb45f653fc/status?branch=master)](https://app.codeship.com/projects/411867)

This demo shows how to build a simple Java project on CodeShip,
with help of Jenkinsfile Runner and a standard [Apache Maven Image pack](https://github.com/oleg-nenashev/jenkinsfile-runner-image-packs/tree/main/maven) offered by the Jenkins project.

In this demo, we have a Pipeline trat...

* Executes Maven Build
* Records Unit test results
* Runs SpotBugs for static analysis and publishes the results

This demo uses [Version Number Library](https://github.com/jenkinsci/lib-version-number) from Jenkins as a target project.
This library does not include any Jenkins-specific code, and can be considered as a simple library written in Java.
  
## TODOs

* Record Coverage
* Publish Build results to build log or to GitHub Actions
* Nice2Have: Maven artifact caching on CodeShip

## License

[MIT License](./LICENSE.txt)


