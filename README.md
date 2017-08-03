# HTTP Hello

Simple http server that returns a `Hello + random name` for test purposes

# Run:
```
mvn spring-boot:run
```

# Build:
```
mvn clean package docker:build
```

# Run Container:
```
docker run -d --name http-hello \
-e SERVER_TOMCAT_ACCESSLOG_ENABLED=true \
-e JAVA_TOOL_OPTIONS="-Xmx512m" \
-p 7777:7777 \
r1ckr/http-hello
```