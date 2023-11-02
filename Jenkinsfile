// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'pwd'
                sh 'ls'
                sh 'npm run currency_breakdown.js'
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
        echo 'Building....'
    }
    stage('Deploy') {
        echo 'Deploying....'
    }
}
