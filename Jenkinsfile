pipeline {
    agent any
     
    stages {
        stage('Ok') {
            steps {
                echo "Ok"
            }
        }
    }
    post {
        always {
            emailext body: 'A Test EMail(4thd)to check if its coming from gitsy', recipientProviders: [[$class: 'DevelopersRecipientProvider'], [$class: 'RequesterRecipientProvider']], subject: 'Test'
        }
    }
}
