pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME' // Assurez-vous que JAVA_HOME est configuré dans Jenkins
        maven 'M2_HOME' // Assurez-vous que M2_HOME est configuré dans Jenkins
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'master', 
                url: 'https://github.com/hwafa/timesheetproject.git'
            }
        }

        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
