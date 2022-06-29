pipeline{
    agent any
    
    tools {
        maven 'Maven_Home'  // pass same name which is define in jenkins global configuration
    }

    stages{
        stage("Test"){
            steps{
                //mvn test
                sh "mvn --version"
                //sh "mvn test"
                echo "========executing A========"
            }
           
        }

        stage("Build"){
            steps{
                //mvn install or package
                //sh "mvn package"
                echo "========executing A========"
            }
           
        }
        stage("Deploy on Test"){
            steps{
                // deploy on container -> plugin
                //deploy adapters: [tomcat9(credentialsId: 'tomcatServerDetails', path: '', url: 'http://44.203.54.137:8081')], contextPath: '/app', war: '**/*war'
                echo "========executing A========"
            }
           
        }
        stage("Deploy on Prod"){
            steps{
                // deploy on container -> plugin 
               // deploy adapters: [tomcat9(credentialsId: 'tomcatServerDetails', path: '', url: 'http://44.203.130.195:8081')], contextPath: '/app', war: '**/*war'
                echo "========executing A========"
            }
           
        }
    }
    post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    }
}
