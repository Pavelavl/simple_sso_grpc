## Simple SSO realization with gRPC

_Here I implemented Single Sign-On (SSO) using gRPC, creating a secure and fast communication channel 
between any system components, providing users with a convenient login without re-authentication._

### Used stack:
- Golang
- SQLite

### Migrations && Launching:
1. `cd .\sso`
2. Run migrations - `go run .\cmd\migrator\main.go --storage-path=./storage/sso.db --migrations-path=./migrations`
3. Edit your config (`config/local.yaml`) file, then run app `go run .\cmd\sso\main.go --config=./config/local.yaml`
