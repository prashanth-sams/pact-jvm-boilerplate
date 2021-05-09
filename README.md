# Pact Boilerplate | spring boot
> Pact based consumer driven contract testing boilerplate on spring boot applications

- Launch Pact Broker in local 
```
docker-compose up
```

http://localhost/


![](https://i.imgur.com/2oDXPRU.png)

### Consumer

```
cd consumer/

mvn clean install
mvn spring-boot:run
```

http://localhost:8080/swagger-ui.html


### Provider

```
cd provider/

mvn clean install
mvn spring-boot:run

mvn pact:verify
```

http://localhost:7073/swagger-ui.html


![](https://i.imgur.com/7l32O4R.png)


### Software specs
**Java**: `< JDK 14`
```
https://download.java.net/java/GA/jdk13.0.2/d4173c853231432d94f001e99d882ca7/8/GPL/openjdk-13.0.2_osx-x64_bin.tar.gz
xattr -r -d com.apple.quarantine /Library/Java/JavaVirtualMachines/jdk-13.0.2.jdk
```
