pipeline {
    agent{
        label "worker1"
    }
    stages{
        stage("stage1"){
            steps{
                sh '''
                echo "this is post example"
                echo "Success, Abort"
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
        abort{
            echo"I cencelled it"
        }
        failure {            echo 'I failed :('        
        }
    }
}
