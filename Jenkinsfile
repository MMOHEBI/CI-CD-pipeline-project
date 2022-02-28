pipeline{
    agent{ // where to execute
        label "node"
    }
    stages{ // where the "work" happens
        stage("build"){
            steps{

                echo "building the application...."
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
    stage("test"){
        steps{
            echo "testing application..."
        }
        post{
            always{
                echo "====++++always++++===="
            }
            success{
                echo "====++++test executed successfully++++===="
            }
            failure{
                echo "====++++test execution failed++++===="
            }
    
        }
    }
}
}