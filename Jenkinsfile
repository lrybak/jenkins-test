properties([
  parameters([
    string(name: 'submodule', defaultValue: 'x'),
    string(name: 'submodule_branch', defaultValue: 'y'),
    string(name: 'commit_sha', defaultValue: 'z'),
  ])
])

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
