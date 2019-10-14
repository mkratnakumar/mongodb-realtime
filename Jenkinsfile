pipeline{
    agent any
    stages{
        stage('Git Checkout'){
            steps{
                git url: 'https://github.com/mkratnakumar/mongodb-realtime.git'
            }
        }
        
        stage('Dev Deploy'){
            steps{
                sh "ansible-playbook -i dev.invenory mongodb.yml"
            }
        }
        
    }
}
