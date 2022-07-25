pipeline{
    agent any

    stages {
        stage("build") {
            steps {
                echo 'Building the app..'
            }
        }
        stage("test") {
            steps {
                echo 'Testing the app..'
            }
        }
        stage("deploy") {
            when{
                expression{
                    env.BRANCH_NAME == main
                }
            }
             steps {
                echo 'Deploying the app..'
             }
        }
    }
    post{
        always {

        }
    }
}