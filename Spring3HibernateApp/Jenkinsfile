pipeline {
    agent any
    stage {
            stage ('compile stage'){
                steps {
                    withMaven(maven : 'maven_3_5_2') {
                        sh 'mvn clean compile'
                    }
                }
            }
    stage ('Testing stage') {
        
                steps {
                    withMaven(maven : 'maven_3_5_2') {
                        sh 'mvn test'
                    }
                }
            }
            
            stage ('Deployment stage') {
        
                steps {
                    withMaven(maven : 'maven_3_5_2') {
                        sh 'mvn test'
                    }
                }
            }
    }   
}
