.PHONY: run

run:
	go run -tags "json1 sqlite3" ./main.go

build:
	mkdir -p bin
	env GOOS=linux GOARCH=arm64 go build -tags "json1 sqlite3" -o bin/focalboard-app
