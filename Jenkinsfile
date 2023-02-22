#!groovy

pipeline {
    agent { node {} }

    stages {

        stage("Build") {
            steps {
                echo "Building..."
                git 'https://gitlab/engineering/automation/create_pass_criteria.git'
                sh './mvnw clean compile'
                git credentialsId: 'f36e2f89-b6b9-4f68-8ee3-3a39c605f667', url: 'https://github.com/rahmafeidi/depot-.git'
            }
          }
      }
    }
