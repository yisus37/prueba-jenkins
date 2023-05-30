pipeline{
    agent{
        label "master"
    }
    environment{
        appName="variables"
    }
    stages{
        stage("paso 1"){
            steps{
                scripts{
                    sh "echo 'Hola Mundo' "
                }
            }
            post{
                always{
                    echo "========always========"
                }
                success{
                    echo "========A executed successfully========"
                }
                failure{
                    echo "========A execution failed========"
                }
            }
        }
    }
/*     post{
        always{
            echo "========always========"
        }
        success{
            echo "========pipeline executed successfully ========"
        }
        failure{
            echo "========pipeline execution failed========"
        }
    } */
}
