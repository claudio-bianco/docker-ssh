pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh 'docker --version'
//                sh 'docker compose build'
                sh 'docker compose up -d'
            }
        }
        stage('ssh') {
            steps {
            sshagent(credentials:['ssh credential']){
//               sh 'ssh -o StrictHostKeyChecking=no root@135.181.203.3 uptime "whoami"'
               sh 'ssh -o StrictHostKeyChecking=no remote-host@remote-host uptime "whoami"'
               }
               echo "success lgoin"
            }
        }        
    }
}