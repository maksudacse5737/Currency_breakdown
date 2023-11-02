// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'building..'
                echo 'schedule added here'
                echo 'changed'
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
        git branch: 'main', url: 'https://github.com/maksudacse5737/Currency_breakdown.git'
        try {
          sh "npm run currency_breakdown.js" 
        } catch (Exception err) {
          currentBuild.result = 'UNSTABLE'
        }
        }
    stage('Deploy') {
        echo 'Deploying....'
    }
}
