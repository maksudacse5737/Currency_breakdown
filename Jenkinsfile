// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/maksudacse5737/Currency_breakdown.git'
                sh 'npm install -g npm@latest'
                sh 'npm cache clean --force'
                sh 'npm rm -rf node_modules && rm package-lock.json'
                sh 'npm install'
                echo 'building..'
                echo 'schedule added here'
                echo 'changed yes'
            }
        }
        stage('Test') {
            steps {
                sh "npm run currency_breakdown.js" 
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
