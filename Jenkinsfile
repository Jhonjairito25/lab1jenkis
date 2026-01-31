pipeline {
    agent any

    stages {
        stage('Probar SSH a GitHub') {
            steps {
                node {
                    powershell """
                    # Configurar la clave SSH
                    \$env:GIT_SSH_COMMAND='ssh -i C:/Users/llano/Documents/lab1jenkis/jenkins_id_rsa -o StrictHostKeyChecking=no'

                    # Probar conexión a GitHub
                    ssh -T git@github.com

                    # Clonar el repositorio para verificar acceso
                    git clone git@github.com:Jhonjairito25/lab1jenkis.git
                    """
                }
            }
        }
    }
}
﻿