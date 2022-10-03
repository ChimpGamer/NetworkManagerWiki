# Gradle

Add these lines to your gradle buildscript in order to use the networkmanager api in your project module(s).

#### Groovy DSL

```groovy
repositories {
    maven { url 'https://repo.networkmanager.xyz/repository/maven-public/' }
}

dependencies {
    compileOnly 'nl.chimpgamer.networkmanager:api:2.12.3'
}
```

#### Kotlin DSL

```kts
repositories {
    maven("https://repo.networkmanager.xyz/repository/maven-public/")
}

dependencies {
    compileOnly("nl.chimpgamer.networkmanager:api:2.12.3")
}
```
