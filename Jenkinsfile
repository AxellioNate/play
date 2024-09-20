pipeline {
    agent {
        label 'build2'
    }


    stages {
        stage('el8') {
            environment {
                BRANCH_NAME="remotes/origin/master"
                BRANCH="remotes/origin/master".replaceAll("^.*/.*/", "")
                BRANCH2=BRANCH_NAME.replaceAll("^.*/.*/", "")
            }
            stages {
                stage('Configure') {
                    steps {
                        sh "echo working in ${BRANCH2}"
                    }
                }
            }
        }
    }
}
