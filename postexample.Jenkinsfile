pipeline {
    agent{
        label "worker1"
    }
    stages{
        stage("stage1"){
            steps{
                sh '''
                echo "this is post example"
                '''
            }
        }
    }
    post{
        always{
            echo "One Way or other I have finished"
        }
        success{
            echo "I succeed"
        }
        
    }
}
