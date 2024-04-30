pipeline{
    agent { label 'mestre' }

    environment{
        PASS = 'senha'
    }

    stages{

        stage('Recuperar Senha Vault'){
            steps{
                sh 'printenv'
            }
        }

        stage('stage2'){
            steps{
                echo 'step 1 do stage 2'
            }
        }
                 
    }
}
