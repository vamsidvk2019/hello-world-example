node('master') {
checkout scm
stage('build') {
    withMaven(jdk: 'Default Java', maven: 'Default Maven') {
        /* .. some comment .. */
    sh 'mvn clean install'
}
}
}
