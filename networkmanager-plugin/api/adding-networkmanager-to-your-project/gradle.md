# Gradle

Add these lines to your gradle buildscript in order to use the networkmanager api in your project module(s).

#### Groovy DSL

```
repositories {
    maven { url 'https://repo.networkmanager.xyz/repository/maven-public/' }
}

dependencies {
    compileOnly 'nl.chimpgamer.networkmanager:api:2.10.4'
}
```

#### Kotlin DSL

```
repositories {
    maven("https://repo.networkmanager.xyz/repository/maven-public/")
}

dependencies {
    compileOnly("nl.chimpgamer.networkmanager:api:2.10.4")
}
```
