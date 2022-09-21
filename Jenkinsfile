pipeline {
    agent any

    stages {
        stage('all') {
            steps {
                sh 'ssh root@172.31.4.233 "yum update -y"'
                sh 'ssh root@172.31.4.233 "amazon-linux-extras install java-openjdk11 -y"'
                sh 'ssh root@172.31.4.233 "wget https://dlcdn.apache.org/tomcat/tomcat-9/v9.0.65/bin/apache-tomcat-9.0.65.tar.gz"'
                sh 'ssh root@172.31.4.233 "tar -xzvf  apache-tomcat-9.0.65.tar.gz"'
                sh 'ssh root@172.31.4.233 "rm -fr  apache-tomcat-9.0.65.tar.gz"'
                sh 'ssh root@172.31.4.233 "mv apache-tomcat-9.0.65 tomcat9"'
                sh 'ssh root@172.31.4.233 "cd tomcat9/bin/ && ./startup.sh"'
                // sh 'ssh root@172.31.4.233 "cd tomcat9"'
                // sh 'ssh root@172.31.4.233 "ls -ltrh"'
                // sh 'ssh root@172.31.4.233 "cd bin"'
                // sh 'ssh root@172.31.4.233 "ls"'
                // sh 'ssh root@172.31.4.233 "chmod 755 *.sh"'
                // sh 'ssh root@172.31.4.233 "/  startup.sh"'
            }
        }
       
    }
}