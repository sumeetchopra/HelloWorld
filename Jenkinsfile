pipeline {
   agent any
   properties([parameters([string(defaultValue: '', description: '', name: 'checkParam')]), pipelineTriggers([])])
   stages {
     stage('Build') {
         steps {
             sh 'echo "Hello World"'
             sh '''
                 echo "Multiline shell steps works too"
                 ls -lah
             '''
         }
     }

     stage('TestCheckParam') {
        steps {
         echo "${params.checkParam} World!"
        }
     }

   }
}
