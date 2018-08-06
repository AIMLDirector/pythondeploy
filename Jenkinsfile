node {
        stage("Main build") {
            checkout scm

            docker.image('python').withRun('-u root --name testnode') {

              stage("Install Tomcat") {
                sh "pip install version"
              }
            

           }

        }

        // Clean up workspace
        step([$class: 'WsCleanup'])

}
