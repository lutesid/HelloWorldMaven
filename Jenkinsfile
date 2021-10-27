pipeline { 
    agent any 
    stages {
        stage('Build') { 
            steps {
                withMaven(maven : 'Apache_Maven_3.5.4'){
                        sh "mvn clean compile"
                } 
            }
        }
        stage('Test'){
            steps {
                withMaven(maven : 'Apache_Maven_3.5.4'){
                        sh "mvn test"
                }

            }
        }

    }
}
