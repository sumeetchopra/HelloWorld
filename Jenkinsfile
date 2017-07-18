pipeline {
    agent any
    parameters {
        string(name: 'checkParam', defaultValue: '', description: '')
    }
    stages {
        stage('disp') {
            steps {
                echo "${params.checkParam} World!"
            }
        }
    }
}
