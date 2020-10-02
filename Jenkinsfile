pipeline {
    agent none
    tools {
        maven "mvn"
        jdk 'jdk8'
    }
    options {
        // Not used in Jenkinsfile Runner
        buildDiscarder(logRotator(numToKeepStr: '10'))
    }
    stages {
        stage('Linux') {
            agent {
                label "linux"
            }
            steps {
                sh 'mvn -V -B -Dmaven.test.failure.ignore=true clean verify'
                junit '**/target/surefire-reports/TEST-*.xml'
                recordIssues(
                    enabledForFailure: true, aggregatingResults: true, 
                    tools: [java(), spotBugs(pattern: '**/target/findbugsXml.xml')]
                )
            }
        }
    }
}
