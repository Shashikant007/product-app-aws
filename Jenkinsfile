//Jenkins pipeline
pipeline {
agent any
environment {
    JAVA_HOME="C:/jdk-21.0.7/jdk-21.0.7_windows-x64_bin/jdk-21.0.7"
  }
stages {
 
stage('GIT Repository Download') {
steps {
bat 'git clone https://github.com/Shashikant007/product-app-aws'
dir("product-app-aws") {
bat 'git pull'
}
}
}    
stage('Clean stage') {
steps {
dir("Shashikant007/product-app-aws") {
bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn clean'
}
}
}
 
stage('Compile stage') {
steps {
dir("Shashikant007/product-app-aws") {
bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn compile'
}
}
}
 
stage('Install stage') {
steps {
dir("Shashikant007/product-app-aws") {
bat 'C:/apache-maven-3.9.11-bin/apache-maven-3.9.11/bin/mvn install'
}
}
}
 
}
}
