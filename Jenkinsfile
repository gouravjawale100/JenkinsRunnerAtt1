pipeline {
    agent any

    stages {
        stage('checkout first repo') {
            steps {
                dir('SCM1')
                {
                git 'https://github.com/Vimannagar/ATT30SeptBDDBasics'
                }
            }
        }
        
    stage('checkout second repo') {
            steps {
                
                dir('SCM2')
                {
                git 'https://github.com/gouravjawale100/ATT18NovBDDProject'
                }
        }
        }
        
     stage('build first repo') {
            steps {
               
                    bat "mvn -f ./SCM1 clean test"
                
            }
        }    
    }
}
