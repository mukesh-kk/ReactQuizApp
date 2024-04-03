pipeline{
    agent any
    stages {
        stage('build') {

            steps {
                sh 'npm i -f && npm run build'
            }
           
        }
        stage('deploy') {
            steps {
                sh 'serve -s build'
            }
        }
    }
}