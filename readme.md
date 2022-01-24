### Install CLI
https://github.com/golang-migrate/migrate/edit/master/cmd/migrate/README.md

### Create Migration
```bash
migrate create -ext sql -dir db/migrations -seq create_users_table
```
### Run Migration
```bash
migrate -database 'postgres://postgres:password@localhost:9432/golang_migration?sslmode=disable' -path db/migrations up
```
Or 
```bash
go run .
```