.PHONY: run

run:
	go run -tags "json1 sqlite3" ./main.go

build:
	mkdir -p bin
	env GOOS=linux GOARCH=arm64 CGO_ENABLED=1 CC=/usr/bin/aarch64-linux-gnu-gcc go build -tags "json1 sqlite3" -o bin/focalboard-app
