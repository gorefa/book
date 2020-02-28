# golang

#### test

## \# test

```text
test

```

{% code title="main.go" %}
```go
package main

import "fmt"

// value,ok := x.(T)
// x表示一个接口的类型，T表示一个类型（也可为接口类型）

// 该断言表达式会返回x的值和一个布尔值 可根据该布尔值判断x是否为T类型

func main() {
	var a int
	a = 10
	judgeType(a)
}

func judgeType(a interface{}) {
	switch a.(type) {
	case int:
		fmt.Println("int")
	case string:
		fmt.Println("string")
	case float64:
		fmt.Println("float")
	default:
		fmt.Println("unknown type")
	}
}

```
{% endcode %}



