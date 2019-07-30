pipeline {
    agent any

    tools{
       maven 'M3'
       docker 'docker' 
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
        
