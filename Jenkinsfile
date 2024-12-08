pipeline {
    agent any

    stages {
        stage('Job 1: Clone Repository') {
            steps {
                // Clone the GitHub repository
                git branch: 'master', url: 'https://github.com/Abhinaybethi/week5new.git'
            }
        }

        stage('Job 2: Execute Java Program') {
            steps {
                script {
                    // Compile and run the Java program
                    bat '''
                    javac helloworld.java
                    java helloworld
                    '''
                }
            }
        }

        stage('Job 3: Execute Python Program') {
    steps {
        script {
            // Check if the Python file exists
            bat 'dir helloworld.py'
            
            // Execute the Python program
            bat 'python helloworld.py'
        }
    }
}
    }
}
