//Jenkins pipeline
pipeline {
agent any
environment {
    JAVA_HOME="C:/jdk-21.0.7/jdk-21.0.7_windows-x64_bin/jdk-21.0.7"
  }
stages { 
stage('Clean stage') {
steps {
bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn clean'

}
}
 
stage('Compile stage') {
steps {
bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn compile'
}
}
 
stage('Install stage') {
steps {

bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn install'

}
}
 
}
}
