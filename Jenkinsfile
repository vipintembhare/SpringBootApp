pipeline {
    agent any

    tools{
       maven 'M3'
    }
    stages {
         stage ('Pull') {

            steps {
               git url: 'https://github.com/vipintembhare/SpringBootApp.git'
            }
        }
        stage ('Compile Stage') {

            steps {
                    sh 'mvn clean install'
            }
        }
    }
}
        
