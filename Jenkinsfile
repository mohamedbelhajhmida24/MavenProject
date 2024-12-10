pipeline {
agent any
tools{ jdk 'jdk19' }
environment { JAVA_HOME = 'C:\\Program Files\\Java\\jdk-19' }
stages {
stage ('Compile Stage') {
steps {
withMaven(maven : 'maven-3.9.9') {
bat 'mvn clean compile'
}

}
stage ('Testing Stage') {

steps {
withMaven(maven : 'maven-3.9.9') {
bat 'mvn test'
} }}
stage ('Install Stage') {
steps {
withMaven(maven : 'amaven-3.9.9') {
bat 'mvn install'
} } } }}
