pipeline{
    agent { label 'mestre' }

    environment{
        PASS = 'senha'
    }

    stages{

        stage('Recuperar Senha Vault'){
            steps{
                sh '''
                    PASS=$(vault kv get -field "VIASOFT" -address="http://vault.viasoftcloud.com.br:8200" VIASOFT/ACAR/ORACLE/AGROTITAN/acar)
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
