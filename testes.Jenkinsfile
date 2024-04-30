pipeline{
    agent { label 'mestre' }

    environment{
        PASS = 'senha'
    }

    stages{

        stage('Recuperar Senha Vault'){
            steps{
                sh '''
                    PASS=$(date)
                '''
            }
        }
                
    }
}