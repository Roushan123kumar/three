# three






mvn --version
mvn archetype:generate 

cd sample-app
app.java->BankService.java
mvn clean
mvn package

cd target
java -cp sample-app-1.0-SNAPSHOT.jar com.bnmit.BankService
