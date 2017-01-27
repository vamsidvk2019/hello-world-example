node('master') {
checkout scm
stage('build') {
    withMaven(jdk: 'Default Java', maven: 'Default Maven') {
        # added a comment
    sh 'mvn clean install'
}
}
}
