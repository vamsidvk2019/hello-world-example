node('master') {
stage('scm') {
    checkout([$class: 'GitSCM', branches: [[name: '']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'github-jenkins-ssh-key', url: 'git@github.com:pro-continuous-delivery/hello-world-example.git']]])
}
stage('build') {
    withMaven(jdk: 'Default Java', maven: 'Default Maven') {
    sh 'mvn clean install'
}
}
}
