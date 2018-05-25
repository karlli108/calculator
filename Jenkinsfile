pipeline {
    agent {
        docker {
            image 'gradle'
        }
    }
    stages {
        stage("Compile"){
            steps {
               sh "./gradlew compileJava" 
            }
        }
        stage('Test'){
            steps {
                sh "./gradlew test"
            }
        }
    }
}
