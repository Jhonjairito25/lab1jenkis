pipeline {
    agent any

    stages {
        stage('Probar SSH a GitHub') {
            steps {
                sshagent(['git']) { 
                    powershell '''
                        ssh -i C:/Users/llano/Documents/lab1jenkis/jenkins_id_rsa -o StrictHostKeyChecking=no git@github.com
                    '''
                }
            }
        }
    }
}
