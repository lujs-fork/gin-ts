```go
func main() {
	r := gin.Default()
	r.GET("/ping", func(c *gin.Context) {
		c.JSON(200, gin.H{
			"message": "pong",
		})
	})
	r.Run() // listen and serve on 0.0.0.0:8080
}
```

```ts
function main() {
	const r = new Gin()
	r.GET("/ping", function(c: Context) {
		c.JSON(200, 
			"message": "pong",
		})
	})
	r.Run() // listen and serve on 0.0.0.0:8080
}
```