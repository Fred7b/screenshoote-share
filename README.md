# screenshoote-share
# Build
1. Install Go 1.16
2. git clone repo & cd screenshoot-share
3. 
```shell
go mod vendor
```
4.Change const in client/app.go
```go
const (
	downloadScript string = "http://localhost:8081/download/"
	uploadScript   string = "http://localhost:8081/upload"
)
```
5. Run make
> linux server Build
```shell
make build_linux_server
```
> linux Build
```shell
make build_linux
```
 > win Build
```shell
make build_win
```
> mac Build
```shell
make build_mac
```
6. Для запуска бинарника под мак следует выдать права
 > System Preferences -> Security & Privacy -> Screen Recordong -> через + добавить приложение в список разрешенных.
 > Если запускается из terminal, то разрешить Teminal / iTerm