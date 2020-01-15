# HTTP Hello

Simple http server that returns a `Hello + random name` for test purposes

# Run:
```
node server.js
```

# Build:
```
docker build . -t r1ckr/http-hello:${version}
```

# Run Container:
```
docker run -d --name http-hello \
-p 7777:7777 \
r1ckr/http-hello
```