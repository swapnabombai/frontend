pipeline {
    agent {
      node { label 'practice' }

    }




        stage('unit tests') {
           steps {
                echo 'unit tests'
                // sh 'npm test'
           }
        }

        stage('code analysis') {
           steps {
               sh 'sonar-scanner -Dsonar.host.url=http://172.31.80.223:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=frontend'
           }
        }

        stage('Security Scans') {
           steps {
               echo 'Security Scans'
           }
        }

        stage('Publish a Artifact') {
           steps {
               echo 'Publish a Artifact'
           }
        }
    }
}