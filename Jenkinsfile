pipeline{
    
    agent any
    
    stages{
        stage('Start') {
            steps {
                echo '?? Pipeline started by Poll SCM!'
                echo "Time: ${new Date()}"
            }
        }
        stage("code clone"){
            steps {
                echo "clone the code"
            }
        }
        stage("test"){
            steps {
                echo "test the code"
            }
        }
        stage("file"){
            steps {
                sh 'ls -llah'
                echo 'check all files'
            }
        }
        stage("deploy"){
            steps {
                echo "deploy to k8s"   
            }
        }
    }
}