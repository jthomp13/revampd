#MAKEFLAGS += --silent

all: clean test build

test:
	GOLANG_ENV=test go test -coverprofile=coverage.txt -covermode=atomic -cover github.com/USEPA/revampd/src

build:
	go build -o ../bin/revampd

clean:
	rm -f ../bin/revampd coverage.txt
