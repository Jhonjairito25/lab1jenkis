pipeline {
    agent any

    stages {
        stage('Hola PowerShell') {
            steps {
                // Esto se ejecuta dentro de un nodo (workspace)
                powershell '''
                    Write-Host "Hola desde PowerShell en Jenkins"
                '''
            }
        }
    }
}
