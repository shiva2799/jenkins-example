// pipeline {
//     agent any

//     stages {
//         stage ('Compile Stage') {

//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn clean compile'
//                 }
//             }
//         }

//         stage ('Testing Stage') {

//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn test'
//                 }
//             }
//         }


//         stage ('Deployment Stage') {
//             steps {
//                 withMaven(maven : 'maven_3_5_0') {
//                     sh 'mvn deploy'
//                 }
//             }
//         }
//     }
// }

pipeline {

    agent any
    tools {
        maven 'mvn' 
    }
    stages {
        stage('Compile stage') {
            steps {
                bat "mvn clean compile" 
        }
    }

         stage('testing stage') {
             steps {
                bat "mvn test"
        }
    }

 // cannot deploy as techprimer has different account on the hosting platform and I don't have the credentials
//           stage('deployment stage') {
//               steps {
//                 bat "mvn deploy"
//         }
//     }

  }

}
