pipeline{
    agent any
    states{
        stage("checkout"){
            steps{
                checkout scm
            }
        }

        stage("Test"){
            steps{
                sh 'sudo npm install'
                sh 'npm test'
            }
        }

        stage("Build"){
            steps{
                sh `npm run build`
            }
        }

    }
}