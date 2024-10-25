properties([
  parameters([
    string(name: 'submodule', defaultValue: 'x'),
    string(name: 'submodule_branch', defaultValue: 'y'),
    string(name: 'commit_sha', defaultValue: 'z'),
    activeChoice(choiceType: 'PT_SINGLE_SELECT'
                  description: 'desc',
                 filterLength: 1, filterable: false, name: 'myparam', randomName: 'choice-sth'
                 script: gtoovyScript(
                   fallbackScript: [classpath: [],
                                    oldScript: '',
                                    sandbox: false, script: 'return false'],
                   script: [classpath: [], oldSscript: '', sandbox: false, script: 'return ["aa"]']
                   )
                 )
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
