EDIT - IDE fault?: Someone has since told me to use `java -cp target/untitled-1.0-SNAPSHOT/WEB-INF/classes:target/untitled-1.0-SNAPSHOT/WEB-INF/lib/*.jar org.cor.lan.WebServer` in Github Codespaces and it worked. I could not replicate this in my IntelliJ IDE.

This repository has been made public to provide 'helpers' access to the code I'm experiencing problems on.

Steps to recreate: <br/>
1: `mvn clean package` to create the .war file <br/>
2: `java -jar target/untitled-1.0-SNAPSHOT.war` to try run said file<br/>
Result: 
```
Error: Could not find or load main class org.cor.lan.WebServer
Caused by: java.lang.ClassNotFoundException: org.cor.lan.WebServer
