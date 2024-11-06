.PHONY: run

run:
	go run -tags "json1 sqlite3" ./main.go

build:
	mkdir -p bin
	env GOOS=linux GOARCH=arm64 CGO_ENABLED=1 CC=/usr/bin/aarch64-linux-gnu-gcc go build -ldflags '-X "github.com/mattermost/focalboard/server/model.BuildNumber=11688994561" -X "github.com/mattermost/focalboard/server/model.BuildDate=Tue Nov  5 17:03:46 UTC 2024" -X "github.com/mattermost/focalboard/server/model.BuildHash=d3aa944cd57d39d59d36dda3d03c2f77016c1e59" -X "github.com/mattermost/focalboard/server/model.Edition=linux"' -tags "json1 sqlite3" -o bin/focalboard-app
