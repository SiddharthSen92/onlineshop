node{

    stage('SCM Checkout')
    {
        git 'https://github.com/SiddharthSen92/onlineshop.git'
    }
    
    stage('Run Docker Compose File')
    {
        sh 'docker-compose build'
        sh 'docker-compose down'
        sh 'docker-compose up -d'
    }
    
    stage('Push Docker Image to HUB')
    {
        sh 'docker push sidrex/firstproject'
    }
    
}
