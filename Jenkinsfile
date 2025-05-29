// pipeline {
//     agent {
//         node {
//             label 'maven'
//         }
//     }
//     environment {
//         PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
//     }
//     stages {
//         stage ("build") {
//             steps {
//                 sh "mvn clean deploy"
//             }
//         }
//     // stage('SonarQube analysis') {
//     // environment {
//     //     scannerHome = tool 'valaxy-sonar-scanner'
//     // }
//     // steps{
//     // withSonarQubeEnv('valaxy-sonarqube-server') {
//     //     sh"${scannerHome}/bin/sonar-scanner"
//     //         }
//     //     }
//     //     }
//     }
// }
// pipeline {
//     agent {
//         node {
//             label 'maven'
//         }
//     }
    
//     stages {
//         stage ('Clone-code') {
//             steps {
//                 git branch: 'main', url: 'https://github.com/Alpha6677/ttrend.git'
//             }
//         }
//     }
// }

pipeline {
    agent {
        node {
            label 'maven'
        }
    }
    environment {
        PATH = "/opt/apache-maven-3.9.9/bin:$PATH"
    }
    stages {
        stage ("build") {
            steps {
                sh "mvn clean deploy"
            }
        }
    }
}