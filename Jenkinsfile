// Declarative //
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/maksudacse5737/Currency_breakdown.git'
                sh 'npm cache clean --force'
                sh 'npm rm -rf node_modules && rm package-lock.json'
                sh 'npm install'
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
                sh 'node currency_breakdown.js'
            }
        }
    }
}
// Script //
// node {
//     stage('Build') {
//         echo 'Building....'
//     }
//     stage('Test') {
//            echo 'Testing....'
//         }
//     stage('Deploy') {
//         echo 'Deploying....'
//     }
// }
