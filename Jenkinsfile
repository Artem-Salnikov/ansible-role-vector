pipeline {
   agent { node { label 'Agent' } }

    stages {
       // stage('Git clone') {
        //    steps {
        //        git branch: 'main', credentialsId: '1c3fc185-e8ee-4165-b376-40f617d13e27', url: 'git@github.com:Artem-Salnikov/ansible-role-vector.git'
        //    }
        //}    
        stage('Molecule test') {
            steps {
                sh 'molecule test -s docker'
            }
        }
    }
}
