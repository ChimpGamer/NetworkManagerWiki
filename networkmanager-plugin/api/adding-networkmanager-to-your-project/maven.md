# Maven

Add these lines to your maven pom file in order to use the networkmanager api in your project module(s).



```xml
    <repositories>
        <repository>
            <id>networkmanager-repo</id>
            <url>https://repo.networkmanager.xyz/repository/maven-public/</url>
        </repository>
    </repositories>
    <dependencies>
        <dependency>
         <groupId>nl.chimpgamer.networkmanager</groupId>
          <artifactId>api</artifactId>
          <version>2.12.3</version>
         <scope>provided</scope>
        </dependency>
    </dependencies>
```
