pipeline{
    agent { label 'mestre' }

    environment{
        PASS = 'senha'
    }

    stages{

        stage('stage1'){
            environment{
                VAR_LOCAL = 'VARIÁVEL LOCAL'
            }
            steps{
                echo 'stage 1'
                sh 'printenv'
            }
        }

        stage('stage2'){
            steps{
                echo 'step1 do stage 2'
            }
        }
                 
    }
}
