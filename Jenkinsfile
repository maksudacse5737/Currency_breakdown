// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/maksudacse5737/Currency_breakdown.git'
                sh "npm run currency_breakdown.js" 
                echo 'building..'
                echo 'schedule added here'
                echo 'changed yes'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
// Script //
node {
    stage('Build') {
        echo 'Building....'
    }
    stage('Test') {
           echo 'Testing....'
        }
    stage('Deploy') {
        echo 'Deploying....'
    }
}
