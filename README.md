CodeShip Demo - Building Java project with Jenkinsfile Runner
====

This demo shows how to build a simple Java project on CodeShip,
with help of Jenkinsfile Runner and a standard [Apache Maven Image pack](https://github.com/oleg-nenashev/jenkinsfile-runner-image-packs/tree/main/maven) offered by the Jenkins project.

In this demo, we have a Pipeline trah...

* Executes Maven Build
* Records Unit test results
* Runs SpotBugs for static analysis and publishes the results

This demo uses [Version Number Library](https://github.com/jenkinsci/lib-version-number) from Jenkins as a target project.
This library does not include any Jenkins-specific code, and can be considered as a simple library written in Java.

## TODOs

* Record Coverage
* Publish Build results to build log or to GitHub Actions

## License

[MIT License](./LICENSE.txt)
