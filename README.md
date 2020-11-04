CodeShip Demo - Building a Java project with Jenkinsfile Runner
====

[![Codeship Status for codeship/codeship-jenkinsfile-java-maven-demo](https://app.codeship.com/projects/6f090f0d-54d5-49f2-b1a1-9757544df513/status?branch=master)](https://app.codeship.com/projects/417038)

This demo shows how to build a simple Java project on CodeShip Pro,
with Jenkins Pipeline and the experimental image designed specially for executions on CodeShip. 

In this demo, we have a Pipeline that...

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


