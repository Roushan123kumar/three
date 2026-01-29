# three

mvn --version
mvn archetype:generate 

cd sample-app
app.java->BankService.java
mvn clean
mvn package

cd target
java -cp sample-app-1.0-SNAPSHOT.jar com.bnmit.BankService


pipeline {
    agent any 

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...' 
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the application...'
                
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
               
            }
        }
    }
}
