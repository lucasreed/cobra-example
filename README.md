Example use of the Cobra tool + package
===

The commands to create this repository are below:

```bash
cobra init --pkg-name github.com/lucasreed/cobra-example -a "Luke Reed" cobra-example
cd cobra-example
cobra add -a "Luke Reed" start
cobra add -a "Luke Reed" stop
go mod init github.com/lucasreed/cobra-example
go mod tidy
```

Then you get the fun of implementing what the actual start and stop commands do, but by default they will print out the fact that they were called:
```
go run main.go start
start called
```