// // Add library from git
// library identifier: 'jenkins-shared-library@master', retrieve: modernSCM(
//     [
//         $class: 'GitSCMSource',
//         remote: 'https://github.com/tieungao88/jenkins-share-lib.git'
//         // credentialsId: 
//     ]
// )
// Add library from jenkin global config
@Library('jenkins-share-lib')
def gv

pipeline {
    agent none
    stages {
        stage("build-docker") {
            echo "Building docker image"
            // agent {
            //     docker { image 'node:13-alpine' }
            // }
            agent 123
            steps {
                script {
                    buildImage "todolist-app"
                }
            }
            echo "Build Done"
        }
    }   
}
