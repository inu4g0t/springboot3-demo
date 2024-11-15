# Init
Init with spring-boot.

# Native image support

ref: https://docs.spring.io/spring-boot/how-to/native-image/developing-your-first-application.html

## add following build plug-in in pom
```
<plugin>
<groupId>org.graalvm.buildtools</groupId>
<artifactId>native-maven-plugin</artifactId>
</plugin>
```

## use native build command(docker is required)
mvn -Pnative spring-boot:build-image