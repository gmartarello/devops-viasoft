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

        stage('Recuperar Senha Vault - 2'){
            steps{
                withVault(configuration: [disableChildPoliciesOverride: false, engineVersion: 2, skipSslVerification: true, timeout: 60, vaultCredentialId: 'vault-read-token', vaultUrl: 'http://vault.viasoftcloud.com.br:8200']) {
                }
            }
        }        
                
    }
}