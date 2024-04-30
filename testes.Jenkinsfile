pipeline{
    agent { label 'mestre' }

    environment{
        PASS = 'senha'
    }

    stages{

        stage('Recuperar Senha Vault'){
            steps{
                sh '''
                    date
                '''
            }
        }

        stage('stage2'){
            steps{
                echo 'step 1 do stage 2'
            }
        }
                 
    }
}
