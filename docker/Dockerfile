# Lightweight alpine OS, weight only 5mb, everything else is Go # # environment
# go language V 1.11.5 support
FROM golang:1.11.5

# Define working directory
WORKDIR /go/src/github.com/luchen29/around

# Add files from your laptop to WORKDIR inside the docker image
ADD . /go/src/github.com/luchen29/around

# Install dependencies
RUN go get -v \
cloud.google.com/go/bigtable \
cloud.google.com/go/storage \
golang.org/x/oauth2/google \
github.com/auth0/go-jwt-middleware \
github.com/dgrijalva/jwt-go \
github.com/go-redis/redis \
github.com/gorilla/mux \
github.com/olivere/elastic \
github.com/pborman/uuid \
gopkg.in/olivere/elastic.v6

# Expose port
EXPOSE 8080

# Entrypoint
CMD ["/usr/local/go/bin/go", "run", "user.go", "main.go", "predict.go"]
