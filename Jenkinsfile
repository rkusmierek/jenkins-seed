pipelineJob('pipeline') {
    definition {
        cpsScm {
            scriptPath 'Jenkinsfile'
            scm {
              git {
                  remote { url 'https://github.com/rkusmierek/spin-kub-demo.git' }
                  branch '*/master'
                  extensions {}
              }
            }
        }
        triggers {
          githubPush()
        }
    }
}