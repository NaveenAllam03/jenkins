

pipeline {
    agent { //adding agent , can add multiple agents
        node {
            label 'agent-1'
        }
    }  
    // build section, Write alll the build steps here 
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
         stage('hi') {
            steps {
                echo 'good morning'
            }
        }
         stage('He') {
            steps {
                echo 'Hello World'
            }
        }
    }
    // Post build section, write what you want to do after build is sucessful
    post {
        always { //multiple options avaliable instead of always, it will run irrespective of results
            echo 'I will always say hello again'
        }
        failure {
            echo 'this runs when pipeline is failes' // generally used when pipiline fails for failure
        }
        sucess {
            echo 'executes when pipeline is sucessful' // runs only when pipeline is sucessful
        }
    }
}
