pipeline {
    agent {
        label "docker-agent"
    }

    triggers {
        pollSCM "* * * * *"
    }
    
    stages {
        stage("Build"){
            steps {
                echo "Building Stage Started"
                sh '''
                    echo "Building processing..."
                '''
            }
        }
        
        stage("Test"){
            steps {
                echo "Test Stage Started"
                sh '''
                    echo "Running tests..."
                '''
            }
        }
        
        stage("Deploy"){
            steps {
                echo "Deployement Stage Started"
                sh '''
                    echo "Deploying..."
                '''
            }
        }
    }
}
